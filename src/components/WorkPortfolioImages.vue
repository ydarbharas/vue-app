<template>
<div class="portfolio__work">
   <div v-for="image in images" :class="image.imageClass" class="portfolio__work__card">
                <img :src="image.imageLink" class="portfolio__work__card__image">
                <div class="portfolio__work__card--overlay">
                    <div class="portfolio__work__card--overlay__hover-icon"><img src="../assets/pe-7s-look.png"></div>
                </div>
            </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            images: [
                {id: 1, imageLink: require("../assets/portfolio-1.jpg"), imageClass: "portfolio__work--column-1 portfolio__work--row-1"},
                {id: 2, imageLink: require("../assets/portfolio-2.jpg"), imageClass: "portfolio__work--column-2 portfolio__work--row-2"},
                {id: 3, imageLink: require("../assets/portfolio-3.jpg"), imageClass: "portfolio__work--column-3 portfolio__work--row-1"},
                {id: 4, imageLink: require("../assets/portfolio-4.jpg"), imageClass: "portfolio__work--column-4 portfolio__work--row-2"},
                {id: 5, imageLink: require("../assets/portfolio-5.png"), imageClass: "portfolio__work--column-1 portfolio__work--row-1"},
                {id: 6, imageLink: require("../assets/portfolio-6.jpg"), imageClass: "portfolio__work--column-2 portfolio__work--row-2"},
                {id: 7, imageLink: require("../assets/portfolio-7.jpg"), imageClass: "portfolio__work--column-3 portfolio__work--row-1"},
                {id: 8, imageLink: require("../assets/portfolio-8.jpg"), imageClass: "portfolio__work--column-4 portfolio__work--row-2"}
            ]
        }
    }
}

</script>

<style lang="scss">
    
@import '../style/variables.scss';
@import '../style/_mixins.scss'; 

.portfolio__work {
    @include gridOctoColumns();
    background-color: $themeColorGrey;
}
    
.portfolio__work--row-1 {
    margin-bottom: -23px;
}

.portfolio__work--row-2 {
    margin-bottom: -31px;
}
    
.portfolio__work--column-1 {
    grid-column: 1 / 3;
}

.portfolio__work--column-2 {
    grid-column: 3 / 5;
}

.portfolio__work--column-3 {
    grid-column: 5 / 7;
}

.portfolio__work--column-4 {
    grid-column: 7 / 9;
}
    
.portfolio__work__card {
    position: relative;
}
  
.portfolio__work__card__image {
    width: 100%
}

.portfolio__work__card--overlay {
   @include overlayImage();
}

.portfolio__work__card:hover .portfolio__work__card--overlay {
    opacity: 0.7;
}
   
.portfolio__work__card--overlay__hover-icon {
    @include centerIcons();
}   
</style>