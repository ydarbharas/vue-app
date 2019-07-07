<template>
    <div>
        <div v-for="stat in stats">
            <img :src="stat.imageLink">
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
                { id: 1, statsNumber: 548, statsAchievement: "projects completed", imageLink: require("../assets/pe-7s-portfolio.png")},
                { id: 2, statsNumber: 1465, statsAchievement: "working hours", imageLink: require("../assets/pe-7s-clock.png")},
                { id: 3, statsNumber: 612, statsAchievement: "positive feedbacks", imageLink: require("../assets/pe-7s-star-white.png")},
                { id: 4, statsNumber: 735, statsAchievement: "happy clients", imageLink: require("../assets/pe-7s-like.png")}
            ]
                    
        }
    }
}
</script>

<style>

</style>