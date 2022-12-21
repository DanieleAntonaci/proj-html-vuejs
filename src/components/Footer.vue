<script>
import JoingForm from './JoingForm.vue';
import NavFooter from './NavFooter.vue';

export default {
    components: { JoingForm, NavFooter },
    data() {
        return {

        }
    },
}
</script>

<template>
    <div>
        <JoingForm/>
        <NavFooter/>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
</style>