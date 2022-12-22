<script>
import AboutUs from './AboutUs.vue';
import Events from './Events.vue';
import HeroesMain from './HeroesMain.vue';
import PresentazioneUniversita from './PresentazioneUniversita.vue'
import UniversityNews from './UniversityNews.vue';

export default {
    components: {
        HeroesMain,
        PresentazioneUniversita,
        AboutUs,
        Events,
        UniversityNews
    }
}
</script>

<template>
    <main >
        <HeroesMain/>

        <PresentazioneUniversita/>

        <!-- linea che divide gli elmenti -->
        <svg class=“fusion-big-triangle-candy” xmlns=“http://www.w3.org/2000/svg” version=“1.1”  viewBox='0 0 100 10'  fill=“rgba(0,0,0)“><path d='M-1 0 L50 6 L101 0 Z'></path></svg>
       
        <AboutUs/>
       
        <Events/>
       
        <UniversityNews/>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

.“fusion-big-triangle-candy” {
    filter: invert(1);
    background-color: #07090a;
    margin-bottom: -5px;
}
</style>