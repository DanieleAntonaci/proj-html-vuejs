<script>
export default {
    data() {
        return {
            ourValues: [
                {
                    text: 'OUR MISSION'
                },
                {
                    text: 'OUR PHILOSOPHY'
                },
                {
                    text: 'OUR COMMITMENT'
                },
                {
                    text: 'OUR PROMISE'
                },
                {
                    text: 'OUR VALUES'
                },
            ],
        }
    },
}
</script>
<template>
    <div id="about-us">
        <div class="container">

            
            <div class="component left">
                <h3>WORLD CLASS FACILITIES</h3>
                <p>Avada University is devoted to excellence in teaching, learning, and research, and developing leaders in many disciplines who make a difference globally.</p>
                <div>
                    <font-awesome-icon icon="fa-solid fa-globe" class="icon"/>
                    <b>International focus</b> - our students come from across the globe
                </div>
                <div>
                    <font-awesome-icon icon="fa-solid fa-graduation-cap" class="icon"/>
                    <b>Residential courses</b> - we encourage learning and growth
                </div>
                <div>
                    <font-awesome-icon icon="fa-regular fa-address-book" class="icon"/>
                    <b>People not profits</b> - education is a right not a privilege
                </div>
                <p>If you prefer to study in your own time and at your own speed then one of our e-learning packages may be right up your street.</p>
            </div>


            <div class="component right">
                <h3>OUR VALUES</h3>
               
                <div class="box" v-for="element in ourValues">
                    <font-awesome-icon icon="fa-solid fa-plus" class="icon"/>
                    {{ element.text }}
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

#about-us {
    background-color: #f7f5f4;
    min-height: 100px;
    padding: 60px 0 100px;

    .container {
        @include flex('only');

        .component {
            width: calc(50% - 20px);


            h3 {
                @include differentFont;
                font-weight: $weight5;
            }

            &.left {
                margin-right: 20px;

                p,
                div {
                    color: $textGray;
                    line-height: 25px;


                }

                p {
                    padding: 15px 0;
                }

                div {
                    padding: 6px 0;

                    .icon {
                        color: $primaryColor;
                        padding-right: 20px;
                    }

                    b {
                        color: black;
                    }
                }

            }

            &.right {
                margin-left: 20px;

                h3 {
                    padding-bottom: 10px;
                }

                .box {
                    width: 100%;
                    padding: 15px;
                    background-color: $thirdColor;
                    color: $primaryColor;
                    margin: 10px 0;

                    &:hover {
                        cursor: pointer;
                    }

                    .icon {
                        padding: 0 15px;
                    }
                }
            }
        }
    }

}
</style>