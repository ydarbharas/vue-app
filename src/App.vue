<template>
    <div id="app">
        <TheNavBar/>
        <HeaderBanner/>
    </div>
</template>

<script>
import HeaderBanner from './components/HeaderBanner.vue'
    
export default {
    components: {
        HeaderBanner 
    }
}
    
</script>

<style>
#app {
text-align: center;
margin: 0px;
 }
</style>