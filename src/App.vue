<script>
import AppMain from './components/AppMain.vue'
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'
export default {
    components: {
        AppHeader,
        AppMain,        
        AppFooter
    }
}
</script>

<template>
    <AppHeader/>
    <AppMain />
    <AppFooter />  
</template>

<style lang="scss">
    @import './style/global.scss';
</style>

