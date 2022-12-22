<script>
export default {
    data() {
        return {
            informations: [
                {
                    text: 'Residential Location 9521 Broadsberry Avenue Paddington RC7 9ZA',
                    link: '#',
                    icon: 'fa-solid fa-house-chimney'
                },
                {
                    text: '1.800.5678910',
                    link: '#',
                    icon: 'fa-solid fa-phone-flip'
                },
                {
                    text: 'info@your-domain.com',
                    link: '#',
                    icon: 'fa-solid fa-envelope'
                },
                {
                    text: 'Monday - Friday: 8:00 AM - 10:00 PM',
                    link: '#',
                    icon: 'fa-regular fa-clock'
                },
            ]
        }
    },
}
</script>

<template>
    <div >
            <h4>AVADA UNIVERSITY</h4>
  
            <a v-for="element in informations" class="contact-university" :href="element.link">
                <font-awesome-icon :icon="element.icon" class="font-icon"/>
                {{ element.text }}
            </a>
            
        </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

div {
    width: calc((100% / 5) - 30px);
    margin: 0 15px;

    h4 {
        padding-bottom: 20px;
    }

    .contact-university {
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

    &.navBrowswer {
        a {
            line-height: 23px;
        }
    }

    #secondNavElement {
        padding-top: 30px;
    }
}
</style>