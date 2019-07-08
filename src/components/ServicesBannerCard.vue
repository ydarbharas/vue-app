<template>
<div class="container services">
    <a name="services"></a>
    <div v-for="service in services" :class="service.serviceClass">
        <img class="icon" :src="service.imageLink">
        <h3 class="service-heading">{{ service.serviceHeading }}</h3>
        <p class="service-text">{{ service.serviceText}}</p>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            services: [
                {id: 1, imageLink: require("../assets/pe-7s-diamond.png"), serviceHeading: "ui/ux design", serviceText: "Be set forth land god darkness make it wherein own", serviceClass: "column-1 row-1"},
                {id: 2, imageLink: require("../assets/pe-7s-arc.png"), serviceHeading: "web development", serviceText: "A she'd them bring void moving third she'd kind fill", serviceClass: "column-2 row-2"},
                {id: 3, imageLink: require("../assets/pe-7s-phone.png"), serviceHeading: "app/mobile", serviceText: "Dominion man second spirit he, earth they're creeping", serviceClass: "column-3 row-1"},
                {id: 4, imageLink: require("../assets/pe-7s-joy.png"), serviceHeading: "game design", serviceText: "Morning his saying moveth it multiply appear life be", serviceClass: "column-4 row-2"},
                {id: 5, imageLink: require("../assets/pe-7s-plane.png"), serviceHeading: "seo/marketing", serviceText: "Give won't after land fill creeping meat you, may", serviceClass: "column-1 row-1"},
                {id: 6, imageLink: require("../assets/pe-7s-star.png"), serviceHeading: "photography", serviceText: "Creepeth one seas cattle grass give moving saw give", serviceClass: "column-2 row-2"},
                {id: 7, imageLink: require("../assets/pe-7s-magic-wand.png"), serviceHeading: "graphic design", serviceText: "Open, great whales air rule for, fourth life whales",  serviceClass: "column-3 row-1"},
                {id: 8, imageLink: require("../assets/pe-7s-paint-bucket.png"), serviceHeading: "illustrations", serviceText: "Whales likeness hath, man kind for them air two won't", serviceClass: "column-4 row-2"}
            ]
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss'; 

.service-heading {
    @include headerFontStyle(); 
    text-transform: uppercase;
    font-size: 12px;
    letter-spacing: 1px;
    padding-top: 10px;
    font-weight: bold;
}
    
.service-text {
    padding: 0px 50px;
    @include textFontStyle();
}

.icon {
    height: 40px;
}
    
.services {
    padding: 70px 10px; 
}
    
.row-1 > p {
     padding-bottom: 50px;   
}
</style>