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

  height: 50px;
  background-color: $primaryColor;

  display: flex;

  .flex-contact-header {
    @include flex('sb-center');

    .list-contact {
      @include flex('only');

      li {
        padding-right: 25px;

        a {
          color: $thirdColor;
          font-size: 14px;

          &:hover {
            text-decoration: underline;
          }

          .font-icon {
            margin-right: 10px;
          }

          .hr-box {
            font-size: 10px;
            background-color: $primaryColor;
            padding: 3px 5px;
            border-radius: 3px;

          }
        }
      }
    }

    .social {
      @include flex('only');

      color: white;
    }
  }
}
</style>