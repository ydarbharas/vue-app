<template>
    <div class="stats__card">
        <div v-for="stat in stats">
            <img class="stats__card__image" :src="stat.imageLink">
            <div class="stats__card__text">
                <h3 class="stats__card__text__numbers">{{ stat.statsNumber }}</h3>
                <p class="stats__card__text__achievement">{{ stat.statsAchievement}}</p>
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

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss';  
        
.stats__card__text__numbers {
    margin-bottom: -10px;
}

.stats__card__text__achievement {
    font-size: 12px;
    font-weight: 500;
    font-weight: bold;
}

.stats__card__image {
    padding-right: 25px;
    padding-top: 20px;
}

.stats__card {
    @include flexCenter();
    font-family: $headerFont;
    padding-top: 75px;
}
    
.stats__card__text {
    float: right;
    letter-spacing: 1px;
    text-transform: uppercase;
    color: $themeColorWhite;
}
</style>