<script>
import AboutUs from './AboutUs.vue';
import HeroesMain from './HeroesMain.vue';
import PresentazioneUniversita from './PresentazioneUniversita.vue'

export default {
    components: {
        HeroesMain,
        PresentazioneUniversita,
        AboutUs
    }
}
</script>

<template>
    <main >
        <HeroesMain/>
        <PresentazioneUniversita/>
        <svg class=“fusion-big-triangle-candy” xmlns=“http://www.w3.org/2000/svg” version=“1.1” width=“100%” height=“10” viewBox='0 0 100 10' preserveAspectRatio=“none” fill=“rgba(0,0,0)“><path d='M-1 0 L50 6 L101 0 Z'></path></svg>
        <!-- <img src="/images/university_ft_bg.png" class="separatore" /> -->
        <AboutUs/>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

.“fusion-big-triangle-candy” {
    filter: invert(1);
    background-color: #07090a;
}
</style>