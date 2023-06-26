<template>
    <div>
        <AppHero/>
        <GameCollection/>
        <AppTeam/>
        <GameMatches/>
        <GameSquads/>
        <AppCommunity/>
        <AppStream/>
        <AppMerch/>
        <GamePartners/>
        <AppPosts/>
        <AppTestimonial/>
    </div>
</template>

<script>
import AppHero from './AppHero.vue';
import GameCollection from './GameCollection.vue';
import AppTeam from './AppTeam.vue';
import GameMatches from './GameMatches.vue';
import GameSquads from './GameSquads.vue';
import AppCommunity from './AppCommunity.vue';
import AppStream from './AppStream.vue';
import AppMerch from './AppMerch.vue';
import GamePartners from './GamePartners.vue';
import AppPosts from './AppPosts.vue';
import AppTestimonial from './AppTestimonial.vue';

export default {
    name: "AppMain",
    
    components: { AppHero,
         GameCollection,
        AppTeam,
        GameMatches,
        GameSquads, 
        AppCommunity, 
        AppStream, 
        AppMerch, 
        GamePartners, 
        AppPosts, 
        AppTestimonial
    }
}
</script>

<style lang="scss" scoped>
    
</style>