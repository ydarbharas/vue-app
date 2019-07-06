<template>
<div>
    <div class="stats-banner">
        <StatisticsBannerCard/>
    </div>
</div>
</template>

<script>
import StatisticsBannerCard from './StatisticsBannerCard.vue'
    
export default {
    data() {
        return {
            stats: [
                { id: 1, statsNumber: 536, statsAchievement: "Projects completed"},
                { id: 2, statsNumber: 243, statsAchievement: "Hours worked"},
                { id: 3, statsNumber: 132, statsAchievement: "Happy customers"}
            ]
                    
        }
    },     
components: {
        StatisticsBannerCard
    }
}
</script>

<style>
.stats-banner {
        background-color: #10c9c3
    }

</style>