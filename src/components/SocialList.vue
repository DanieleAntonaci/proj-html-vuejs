<script>
export default {

}
</script>

<template>
        <ul class="social">
          <li>
            <font-awesome-icon icon="fa-brands fa-facebook-f" />
          </li>
          <li>
            <font-awesome-icon icon="fa-brands fa-twitter"/>
          </li>
          <li>
            <font-awesome-icon icon="fa-brands fa-youtube"/>
          </li>
          <li>
            <font-awesome-icon icon="fa-brands fa-instagram"/>
          </li>  
        </ul>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

li {
  margin-left: 15px;
}
</style>