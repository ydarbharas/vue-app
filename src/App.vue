<template>
    <div id="app">
        <HeaderBanner/>
        <AboutUs/>
    </div>
</template>

<script>
import HeaderBanner from './components/HeaderBanner.vue'
import AboutUs from './components/AboutUs.vue'
    
export default {
    components: {
        HeaderBanner, AboutUs 
    }
}
    
</script>

<style>
#app {
text-align: center;
margin: 0px;
 }
</style>