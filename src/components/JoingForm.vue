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
                <h2>Joing Over
                    <span class="underline">
                        <span class="text">
                            500,000 Students
                        </span>
                        <svg class="line" xmlns=“http://www.w3.org/2000/svg” viewBox='0 0 500 170' preserveAspectRatio=“none”><path d='M8.3,140.2c0,0,200.6-20.6,579-18.8' ></path></svg>
                    </span> 
                Enjoying Avada Education now</h2>
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
                font-weight: 600;

                .underline {
                    color: $primaryColor;
                    display: inline-block;

                    position: relative;

                    .text {
                        position: relative;
                    }

                    .line {
                        position: absolute;
                        position: absolute;
                        top: 37%;
                        left: 50%;
                        width: 220px;
                        height: 80px;
                        transform: translate(-50%, -50%);
                        fill: $primaryColor;


                    }

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