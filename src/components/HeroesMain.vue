<script>
export default {

}
</script>

<template>
    <section id="bg-heroes">
            <h1>Inspiring Tomorrows Leaders</h1>
            <h2>
                The Future Belongs To Those Who See Possibilities Today
            </h2>
            <div>
                <a href="#" class="course">FIND A COURSE</a>
                <a href="#" class="apply">APPLY NOW</a>
            </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

#bg-heroes {
    background-image: url('/images/home_main_slider_bg.jpg');
    min-height: 700px;
    background-position: center;

    @include flex('center');
    flex-direction: column;

    color: $thirdColor;
    line-height: 60px;

    h1 {
        font-size: 60px;
        font-weight: 500;

    }

    h1,
    h2 {
        @include differentFont;
    }

    div {
        margin-top: 10px;

        a {
            color: $thirdColor;
            margin: 20px;
            padding: 10px 20px;
            font-size: 14px;

            &.course {
                background-color: $primaryColor;
            }

            &.apply {
                background-color: $secondaryColor;
            }

            &:hover {
                opacity: .8;
            }
        }
    }
}
</style>