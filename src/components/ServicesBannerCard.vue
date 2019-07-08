<template>
<div class="services__card">
    <div v-for="service in services" :class="service.serviceClass">
        <img class="services__card__icon" :src="service.imageLink">
        <h3 class="services__card__heading">{{ service.serviceHeading }}</h3>
        <p class="services__card__text">{{ service.serviceText}}</p>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            services: [
                {id: 1, imageLink: require("../assets/pe-7s-diamond.png"), serviceHeading: "ui/ux design", serviceText: "Be set forth land god darkness make it wherein own", serviceClass: "services__card--column-1 services__card--row-1"},
                {id: 2, imageLink: require("../assets/pe-7s-arc.png"), serviceHeading: "web development", serviceText: "A she'd them bring void moving third she'd kind fill", serviceClass: "services__card--column-2 services__card--row-2"},
                {id: 3, imageLink: require("../assets/pe-7s-phone.png"), serviceHeading: "app/mobile", serviceText: "Dominion man second spirit he, earth they're creeping", serviceClass: "services__card--column-3 services__card--row-1"},
                {id: 4, imageLink: require("../assets/pe-7s-joy.png"), serviceHeading: "game design", serviceText: "Morning his saying moveth it multiply appear life be", serviceClass: "services__card--column-4 services__card--row-2"},
                {id: 5, imageLink: require("../assets/pe-7s-plane.png"), serviceHeading: "seo/marketing", serviceText: "Give won't after land fill creeping meat you, may", serviceClass: "services__card--column-1 services__card--row-1"},
                {id: 6, imageLink: require("../assets/pe-7s-star.png"), serviceHeading: "photography", serviceText: "Creepeth one seas cattle grass give moving saw give", serviceClass: "services__card--column-2 services__card--row-2"},
                {id: 7, imageLink: require("../assets/pe-7s-magic-wand.png"), serviceHeading: "graphic design", serviceText: "Open, great whales air rule for, fourth life whales",  serviceClass: "services__card--column-3 services__card--row-1"},
                {id: 8, imageLink: require("../assets/pe-7s-paint-bucket.png"), serviceHeading: "illustrations", serviceText: "Whales likeness hath, man kind for them air two won't", serviceClass: "services__card--column-4 services__card--row-2"}
            ]
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss'; 

.services__card {
    @include gridOctoColumns();
    background-color: $themeColorGrey;
    padding: 70px 10px; 
}
    
.services__card__heading {
    @include headerFontStyle(); 
    text-transform: uppercase;
    font-size: 12px;
    letter-spacing: 1px;
    padding-top: 10px;
    font-weight: bold;
}
    
.services__card__text {
    padding: 0px 50px;
    @include textFontStyle();
    padding-bottom: 50px;  
}

.services__card__icon {
    height: 40px;
}
      
.services__card--row-1 {
    margin-bottom: -23px;
}

.services__card--row-2 {
    margin-bottom: -31px;
}
    
.services__card--column-1 {
    grid-column: 1 / 3;
}

.services__card--column-2 {
    grid-column: 3 / 5;
}

.services__card--column-3 {
    grid-column: 5 / 7;
}

.services__card--column-4 {
    grid-column: 7 / 9;
}   
    
</style>