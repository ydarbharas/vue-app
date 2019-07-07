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

<style>
.stats-banner {
    background-color: #10c9c3;
    height: 250px;
    margin-bottom: -20px;
   
    }

</style>