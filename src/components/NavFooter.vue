<script>
import ContactFooter from './ContactFooter.vue';
import CoursesAndAdmissions from './CoursesAndAdmissions.vue';
import FooterRecentPosts from './FooterRecentPosts.vue';
import ResourcesAndQuicklinks from './ResourcesAndQuicklinks.vue';
import UpcomingEvents from './UpcomingEvents.vue';

export default {
    components: { ContactFooter, FooterRecentPosts, CoursesAndAdmissions, ResourcesAndQuicklinks, UpcomingEvents }
}
</script>

<template>
    <div class="cotainerBackground">

        <div id="bottomFooter">
        <ContactFooter/>

        <FooterRecentPosts/>

        <CoursesAndAdmissions/>

        <ResourcesAndQuicklinks/>
   
        <UpcomingEvents/>
       
    </div>
</div>
</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

.cotainerBackground {
    background-image: url('/images/university_ft_bg.png');
    background-position: -250px;


    #bottomFooter {
        max-width: 1300px;
        margin: 0 auto;

        @include flex('s-b');

        padding: 70px 30px 30px;
        font-size: 13px;

        &>div {
            width: calc((100% / 5) - 30px);
            margin: 0 15px;

        }

    }
}
</style>