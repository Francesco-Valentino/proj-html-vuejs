<template>

import Appheader from './Appheader.vue';
    <div>
        <AppHeader/>
        <AppMain/>
        <AppFooter/>
    </div>
</template>

<script>
import AppHeader from './Appheader.vue';
import AppMain from './AppMain.vue';
import AppFooter from './AppFooter.vue';

export default {
    name: "AppWrap",
    
    components: { 
        AppHeader,
        AppMain,
        AppFooter,
    }
}
</script>

<style lang="scss" scoped>
    
</style>