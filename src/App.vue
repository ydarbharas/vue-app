<template>
    <div id="app">
        <HeaderBanner/>
        <AboutUs/>
        <ProfessionalSkills/>
    </div>
</template>

<script>
import HeaderBanner from './components/HeaderBanner.vue'
import AboutUs from './components/AboutUs.vue'
import ProfessionalSkills from './components/ProfessionalSkills.vue'
    
export default {
    components: {
        HeaderBanner, AboutUs, ProfessionalSkills 
    }
}
    
</script>

<style>
#app {
text-align: center;
margin: 0px;
 }
</style>