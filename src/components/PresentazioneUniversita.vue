<script>
export default {

}
</script>

<template>
    <section>
        <div class="container">
            <div class="title">
                <img src="/images/page-logo-1.png" alt="Logo Avada">
                <h2>Inspired By Excellence & Innovation</h2>
                <h3>We offer a wide range of high quality of teaching and extra-curriculum activities.</h3>
            </div>

            <div class="contentDivider"></div>

            <div class="content">
                <div>
                    <h3>WHY CHOOSE AVADA UNIVERSITY?</h3>
                    <p>We offer a range of training packages in a range of subject areas and can offer blended learning opportunities to best meet your needs. If sitting in a room with a trainer and having the opportunity for discussion with other learners sounds good to you then we can offer this. If you prefer to study in your own time and at your own speed then one of our world class facilities.</p>
                    <p>
                    If you prefer to study in your own time and at your own speed then one of our e-learning packages may be right up your street. There is a third option, which is you like the sound of both but perhaps can’t attend all training sessions, this is when blended learning comes into its own.

                    </p>
                </div>
                
                <!-- <iframe width="740" height="360" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" src="https://player.vimeo.com/video/52411719?autoplay=1"></iframe> -->
                <img src="/images/business_seminar_event_feat-400x268.jpg" alt="">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

section {
    padding: 70px 0 60px;

    .title {
        text-align: center;
        margin-top: 40px;

        h2 {
            font-weight: 500;
            padding: 10px 0;
            @include differentFont;
        }

        h3 {
            font-weight: 400;
            color: gray;
        }
    }

    .contentDivider {
        width: 200px;
        border: 1px solid $primaryColor;
        margin: 40px auto;
    }

    .content {
        display: flex;
        justify-content: space-around;

        div {
            margin-right: 70px;

            h3,
            p {
                padding-bottom: 20px;
            }

            h3 {
                @include differentFont;
                font-weight: 500;
            }

            p {
                color: gray;
                line-height: 24px;
                font-size: 14px;
            }
        }

        img {
            height: 200px;
        }

    }
}
</style>