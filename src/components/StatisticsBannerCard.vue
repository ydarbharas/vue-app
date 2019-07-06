<template>
    <div>
        <div v-for="stat in stats">
            <h3 class="stats-number">{{ stat.statsNumber }}</h3>
            <p class="stats-achievement">{{ stat.statsAchievement}}</p>
        </div>
    </div>
</template>

<script>     
export default {
    data() {
        return {
            stats: [
                { id: 1, statsNumber: 536, statsAchievement: "Projects completed"},
                { id: 2, statsNumber: 243, statsAchievement: "Hours worked"},
                { id: 3, statsNumber: 132, statsAchievement: "Happy customers"}
            ]
                    
        }
    }
}
</script>

<style>

</style>