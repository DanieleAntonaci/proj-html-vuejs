<script>
import SocialList from './SocialList.vue';

export default {
    components: { SocialList }
}
</script>

<template>
     <div id="contact-hedaer">
      <div class="container flex-contact-header">
        <ul class="list-contact">
          <li>
            <a href="#">
              <font-awesome-icon icon="fa-solid fa-phone-flip" class="font-icon"/>
                1.800.5678910
                <span class="hr-box">
                  24hrs
                </span>
            </a>
          </li>
          <li>
            <a href="#">
              <font-awesome-icon icon="fa-solid fa-envelope" class="font-icon"/>
                Contact Us
            </a>
          </li>
          <li>
            <a href="#">
              <font-awesome-icon icon="fa-solid fa-graduation-cap" class="font-icon"/>
                Alunni
            </a>
          </li>
          <li>
            <a href="#">
              <font-awesome-icon icon="fa-solid fa-building-columns" class="font-icon"/>
                Campus
            </a>
          </li>
     
        </ul>
     
        <SocialList/>
      </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

#contact-hedaer {
    position: sticky;
    top: 0;
    left: 0;
    height: 50px;
    background-color: $primaryColor;

    display: flex;

    .flex-contact-header {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .list-contact {
            display: flex;

            li {
                padding-right: 25px;

                a {
                    color: white;
                    font-size: 14px;

                    &:hover {
                        text-decoration: underline;
                    }

                    .font-icon {
                        margin-right: 10px;
                    }

                    .hr-box {
                        font-size: 10px;
                        background-color: #e58925;
                        padding: 3px 5px;
                        border-radius: 3px;

                    }
                }
            }
        }

        .social {
            display: flex;
            color: white;


        }
    }
}
</style>