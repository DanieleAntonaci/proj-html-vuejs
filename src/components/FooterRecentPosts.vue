<script>
export default {
    data() {
        return {
            informations: [
                {
                    text: 'What do successful grads think you should study?',
                    date: 'March 16, 2016',
                    link: '#',
                },
                {
                    text: 'Former student discusses success in the fashion industry',
                    date: 'March 15, 2016',
                    link: '#',
                },
                {
                    text: 'How do you best prepare for university?',
                    date: 'March 15, 2016',
                    link: '#',
                }
            ]
        }
    },
}
</script>

<template>
    <div id="recent-posts">
            <h4>RECENT POSTS</h4>
            
            <a v-for="element in informations" :href="element.link">

                <font-awesome-icon icon="fa-solid fa-chevron-right" class="font-icon" />

                <div>
                    
                    {{ element.text }}

                    <span class="date-post">{{ element.date }}</span>

                </div>

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

    a {
        display: flex;
        color: #767e85;
        font-weight: 300;

        &:hover {
            color: $primaryColor;
        }

        .font-icon {
            padding-right: 10px;
        }
    }


    #recent-posts {
        a {
            align-items: baseline;
            padding-top: 10px;

            .font-icon {
                font-size: 10px;
                vertical-align: baseline;
            }

            div {

                line-height: 25px;
                border-bottom: 1px solid #767e85;
                padding-bottom: 10px;
                color: black;

                .date-post {
                    display: block;
                    color: #767e85;
                }
            }
        }
    }
}
</style>