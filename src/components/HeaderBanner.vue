<template>
    <div class="header">
        <HeaderBannerNavigation/>
        <HeaderBannerText/>
    </div>
</template>

<script>
import HeaderBannerNavigation from './HeaderBannerNavigation.vue'
import HeaderBannerText from './HeaderBannerText.vue'
    
export default {
    components: {
        HeaderBannerNavigation, HeaderBannerText
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss'; 
    
.header {
    height: 700px;
    background-color: #dddee3;
    background-image: url(../assets/header-background-image.jpg);
    background-size: contain;
    background-repeat: no-repeat;
    padding: 15px;
}        
</style>