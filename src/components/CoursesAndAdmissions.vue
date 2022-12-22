<script>
export default {
    data() {
        return {
            courses: [
                {
                    text: 'Arts & Humanities',
                    link: '#',
                },
                {
                    text: 'Busines & Menagement',
                    link: '#',
                },
                {
                    text: 'Engineering & Tecnology',
                    link: '#',
                },
                {
                    text: 'Life Sciences & Medicine',
                    link: '#',
                },
                {
                    text: 'Natural Scienses',
                    link: '#',
                },

            ],
            admissions: [
                {
                    text: 'Eligibility',
                    link: '#',
                },
                {
                    text: 'Application',
                    link: '#',
                },
                {
                    text: 'Review Process',
                    link: '#',
                },
                {
                    text: 'How to Apply',
                    link: '#',
                },
            ]
        }
    },
}
</script>

<template>
   <div class="navBrowswer">
            <h4>COURSES</h4>

            <a v-for="element in courses" 
                :href="element.link">   
                {{ element.text }}
            </a>


            <h4 id="secondNavElement">ADMISSIONS</h4>
            
            <a v-for="element in admissions" 
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

    .contact-university {
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
        display: flex;
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