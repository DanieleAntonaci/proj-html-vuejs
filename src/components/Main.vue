<script>
import HeroesMain from './HeroesMain.vue';
import PresentazioneUniversita from './PresentazioneUniversita.vue'

export default {
    components: {
        HeroesMain,
        PresentazioneUniversita
    }
}
</script>

<template>
    <main >
        <HeroesMain/>
        <PresentazioneUniversita/>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
</style>