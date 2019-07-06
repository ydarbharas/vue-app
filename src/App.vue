<template>
    <div id="app">
        <HeaderBanner/>
        <AboutUs/>
        <ProfessionalSkills/>
        <StatisticsBanner/>
    </div>
</template>

<script>
import HeaderBanner from './components/HeaderBanner.vue'
import AboutUs from './components/AboutUs.vue'
import ProfessionalSkills from './components/ProfessionalSkills.vue'
import StatisticsBanner from './components/StatisticsBanner.vue'
    
export default {
    components: {
        HeaderBanner, AboutUs, ProfessionalSkills, StatisticsBanner 
    }
}
    
</script>

<style>
#app {
text-align: center;
margin: 0px;
 }
</style>