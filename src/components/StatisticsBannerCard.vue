<template>
    <div class="stats-card">
        <div v-for="stat in stats">
            <img class="stats-image" :src="stat.imageLink">
            <div class="stats-text">
                <h3 class="stats-numbers">{{ stat.statsNumber }}</h3>
                <p class="stats-achievement">{{ stat.statsAchievement}}</p>
            </div>
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
    
.stats-numbers {
    margin-bottom: -10px;
}

.stats-achievement {
    font-size: 13px;
    font-weight: 500;
}

.stats-image {
    padding-right: 25px;
    padding-top: 20px;
}

.stats-card {
    display: flex;
    justify-content: space-evenly;
    text-align: left;
    padding-top: 75px;
}
    
.stats-text {
    float: right;
    font-family: 'Montserrat', sans-serif;
    letter-spacing: 1px;
    text-transform: uppercase;
    color: #ffff;
}
</style>