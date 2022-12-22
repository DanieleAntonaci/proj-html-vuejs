<script>
import BottomFooter from './BottomFooter.vue';
import JoingForm from './JoingForm.vue';
import NavFooter from './NavFooter.vue';

export default {
    components: { JoingForm, NavFooter, BottomFooter },
    data() {
        return {

        }
    },
}
</script>

<template>
    <footer>
        <JoingForm/>
        <NavFooter/>
        <BottomFooter/>
    </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
</style>