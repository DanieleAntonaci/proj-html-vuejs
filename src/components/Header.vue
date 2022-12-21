<script>
import HeaderListContact from './HeaderListContact.vue';
import NavBarHeader from './NavBarHeader.vue';

export default {
  components: { HeaderListContact, NavBarHeader }
}
</script>

<template>
  <div>
   <HeaderListContact/>
    
   <NavBarHeader/>
  </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
</style>
