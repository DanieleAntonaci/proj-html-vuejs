<script>
export default {
    data() {
        return {
            news: [
                {
                    img: 'news_single_post_header_1-200x111.jpg',
                    title: 'What do successful grads think you should study?',
                    linkAdmin: '#',
                    linkInformation: '#',
                    numMessage: 0,
                    date: 'March 16th, 2016'
                },
                {
                    img: 'news_single_post_header_2-400x222.jpg',
                    title: 'Former student discusses success in the fashion industry',
                    linkAdmin: '#',
                    linkInformation: '#',
                    numMessage: 0,
                    date: 'March 16th, 2016'
                },
                {
                    img: 'news_single_post_header_3-400x222.jpg',
                    title: 'How do you best prepare for university?',
                    linkAdmin: '#',
                    linkInformation: '#',
                    numMessage: 0,
                    date: 'March 16th, 2016'
                },
            ]
        }
    },
}
</script>

<template>
    <section class="newsUniversity">
        <div class="container">

            <div class="title">
                <img src="/images/page-logo-1.png" alt="Logo Avada">
                <h2>Today's University News</h2>
                <h4>Covering Topics From Classes To Politics And Student Organization Events.</h4>
            </div>
            
            <div class="contentDivider"></div>
            
            <div class="cardLink">

                <div class="card" v-for="element in news">
                    <a href="#">
                        <img :src='"images/" + element.img' alt="University News">
                    </a>
                    <div >
                        <a href="#" class="title-card">{{ element.title }}</a>
                        <div class="date">
                            By <a :href="element.linkAdmin">admin</a> {{ element.date }}
                        </div>
                    </div>
                    <div class="readMore">
                        <a :href="element.linkInformation">Reade more 
                            <font-awesome-icon icon="fa-solid fa-angle-right" />
                        </a>
                        <a href="#">
                            <font-awesome-icon icon="fa-regular fa-comments" />
                            {{ element.numMessage }}
                        </a>
                    </div>
                    
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

.newsUniversity {
    background-color: #f7f5f4;
    padding: 90px 0;

    .title {
        text-align: center;
        margin-bottom: 40px;

        h2 {
            @include differentFont;
            font-weight: 500;
            padding: 20px 0;
        }

        h4 {
            font-weight: 300;
            color: $textGray;
        }
    }

    .contentDivider {
        width: 200px;
        border: 1px solid $primaryColor;
        margin: 40px auto;
    }

    .cardLink {

        display: flex;

        .card {
            background-color: $thirdColor;
            width: calc((100% / 3) - 20px);
            color: gray;
            margin: 0 10px;

            @include flex('s-b');
            flex-direction: column;

            a {
                color: $primaryColor;
            }

            img {
                width: 100%;
            }

            &>div {
                padding: 20px;

            }

            .title-card {
                @include differentFont;
            }

            .date {
                font-size: 12px;
                vertical-align: bottom;
                padding-top: 5px;

                a {
                    border-right: 1px solid $textGray;
                    padding-right: 10px;
                }
            }

            .readMore {
                @include flex('s-b');
            }
        }
    }
}
</style>