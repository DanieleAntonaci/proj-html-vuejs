<script>
import HeroesMain from './HeroesMain.vue';

export default {
    components: { HeroesMain }
}
</script>

<template>
    <div >
        <HeroesMain/>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
</style>