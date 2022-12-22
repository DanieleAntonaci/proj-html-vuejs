<script>
export default {
    data() {
        return {
            cards: [
                {
                    text: 'COURSES',
                    link: '#',
                    img: 'home_courses_section_bg.jpg'
                },
                {
                    text: 'EVENTS',
                    link: '#',
                    img: 'home_events_section_bg.jpg'
                },
                {
                    text: 'LATEST NEWS',
                    link: '#',
                    img: 'home_latest_news_section_bg.jpg'
                },
            ]
        }
    },
}
</script>

<template>
    <section id="cards">

        <div class="card" v-for="element in cards">

            <img :src='"/images/" + element.img' :alt="element.text">

            <div class="text">
                <h3>{{ element.text }}</h3>

                <div class="divider"></div>
                
                <a :href="element.link">View More</a>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

#cards {
    min-height: 200px;
    max-width: 1700px;

    .card {
        width: calc(100% /3);
        height: calc(100vw / 3);
        color: $thirdColor;
        position: relative;
        display: inline-block;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);

            text-align: center;

            h3 {
                @include differentFont;
            }

            a {
                color: $thirdColor;
            }


            .divider {
                width: 50px;
                border: 1px solid $primaryColor;
                margin: 40px auto;
            }
        }
    }
}
</style>