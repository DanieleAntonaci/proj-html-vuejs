<script>
import FormRequest from './FormRequest.vue';
export default {
    components: { FormRequest }
}
</script>

<template>
    <div id="upperFooter">
        <div class="container">
            <div class="title-form">
                <h2>Joing Over <span>500,000 Students</span> Enjoying Avada Education now</h2>
                <div>Became Part of Avada University to Further You Career.</div>
                
            </div>
            <FormRequest/>
        </div>
    </div>

</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

#upperFooter {
    background-color: #333c4e;
    min-height: 100px;

    .container {
        padding: 50px 0;
        text-align: center;

        .title-form {
            color: $thirdColor;
            font-family: "Roboto Slab", serif;

            h2 {
                font-weight: 400;

                span {
                    color: $primaryColor;
                }
            }

            div {
                color: gray;
                opacity: .9;
            }

        }

    }
}
</style>