<script>
import BootomFooter from './BootomFooter.vue';
import JoingForm from './JoingForm.vue';
import NavFooter from './NavFooter.vue';

export default {
    components: { JoingForm, NavFooter, BootomFooter },
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
        <BootomFooter/>
    </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
</style>