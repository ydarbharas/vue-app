<template>
    <div class="stats-banner">
        <StatisticsBannerCard/>
    </div>
</template>

<script>
import StatisticsBannerCard from './StatisticsBannerCard.vue'
    
export default {    
    components: {
        StatisticsBannerCard
    }
}
</script>

<style lang="scss">

@import '../style/variables.scss';

.stats-banner {
    background-color: $themeColorBlue;
    height: 250px;
    margin-bottom: -20px;
    }

</style>