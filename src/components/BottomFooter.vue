<script>
import SocialList from './SocialList.vue';

export default {
    components: { SocialList }
}
</script>

<template>
    <div id="container">
        <div>
            <ul>
                <li>
                    <a href="#">&#169; Theme Fusion</a>
                </li>
                <li>
                    <a href="#">All Rights Reseved</a>
                </li>
                <li>
                    <a href="#">Powered by WordPress</a>
                </li>
                <li>
                    <a href="#">support@theme-fusion.com</a>
                </li>
                <li>
                    <a href="#">1.800.555.6789</a>
                </li>
            </ul>

            <SocialList/>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

#container {
    border-top: 1px solid $textGray;

    div {
        @include flex('s-b');
        max-width: 1300px;
        margin: 0 auto;
        padding: 30px;
        font-size: 13px;

        li {
            padding: 0 10px;
            border-right: 1px solid #767e85;
            display: inline;

            &:hover {
                text-decoration: underline;
            }

            a {
                color: $textGray;

            }

            &:last-child {
                border-right: 0;
            }
        }

        .social {
            color: $textGray;
            @include flex('only');
        }
    }
}
</style>