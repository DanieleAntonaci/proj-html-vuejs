
<script>
export default {
    data() {
        return {
            resources: [
                {
                    text: 'Campus Directory',
                    link: '#',
                },
                {
                    text: 'Academic Calendar',
                    link: '#',
                },
                {
                    text: 'Sport Clubs',
                    link: '#',
                },
                {
                    text: 'uate Programs',
                    link: '#',
                },
                {
                    text: 'Faculty & Staff',
                    link: '#',
                },

            ],
            quickLinks: [
                {
                    text: 'University Library',
                    link: '#',
                },
                {
                    text: 'Campus',
                    link: '#',
                },
                {
                    text: 'Careers',
                    link: '#',
                }
            ]
        }
    },
}
</script>

<template>
   <div class="navBrowswer">
            <h4>RESOURCES</h4>

            <a v-for="element in resources" 
                :href="element.link">   
                {{ element.text }}
            </a>


            <h4 id="secondNavElement">QUICKLINKS</h4>
            
            <a v-for="element in quickLinks" 
                :href="element.link">   
                {{ element.text }}
            </a>

        </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

div {
    h4 {
        padding-bottom: 20px;
    }

    &.navBrowswer {
        a {
            line-height: 23px;
        }
    }

    #secondNavElement {
        padding-top: 30px;
    }


    a {
        @include flex('only');
        color: $textGray;
        font-weight: 300;

        &:hover {
            color: $primaryColor;
        }

        .font-icon {
            padding-right: 10px;
        }
    }



}
</style>