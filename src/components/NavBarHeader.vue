<script>
export default {
    data() {
        return {
            navBarArr: [
                {
                    text: 'HOME',
                    link: '#'
                },
                {
                    text: 'ABOUT',
                    link: '#'
                },
                {
                    text: 'COURSES',
                    link: '#',
                    addictionalElement: 'NEW'
                },
                {
                    text: 'EVENTS',
                    link: '#'
                },
                {
                    text: 'FACILITIES',
                    link: '#'
                },
                {
                    text: 'NEWS',
                    link: '#'
                },
                {
                    text: 'ADMISSIONS',
                    link: '#',
                    addictionalElement: 'APPLY'
                },
            ],
            activeItem: 0,
        }
    },
}
</script>

<template>
    <div class="container">
        <div class="nav-bar">
            <a href="#">
                <img src="/images/university_logo.png" alt="Logo Avada Universitry">
            </a>
            <ul>
                <li v-for="(element, index) in navBarArr" >
                    <a :href="element.link" :class="activeItem === index ? 'active' : ''">
                        {{ element.text }}
                    </a>
                    <span v-if="element.addictionalElement" class="addictional-elemnt" >
                        {{ element.addictionalElement }}
                    </span>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;


.nav-bar {
    @include flex('sb-center');

    padding: 10px 0;

    img {
        height: 65px;
    }

    ul {
        @include flex('only');

        li {
            margin-left: 30px;

            a {
                font-weight: $weight5;
                color: black;
                font-size: 13px;

                &:hover {
                    color: $primaryColor;
                }
            }

            .addictional-elemnt {
                margin-left: 10px;
                font-size: 10px;
                vertical-align: middle;
                background-color: $secondaryColor;
                color: $thirdColor;
                padding: 3px 6px;
                border-radius: 3px;
            }

            .active {
                color: $primaryColor;
            }
        }
    }
}
</style>