<template>
    <div class="reviews">
        <a name="testimonials"></a>
        <div id="review">
            <p class="review-text">“ Outstanding job and exceeded all expectations. It was a pleasure to work with them on a sizeable first project and am looking forward to starting the next one asap.”</p>
            <p class="author">Michael Hopkins</p>
        </div>
        <div class="review-icons">
            <img id="review-one" class="review-icon" @click="reviewOne()" src="../assets/carousel-inactive.png">
            <img id="review-two" class="review-icon" @click="reviewTwo()" src="../assets/carousel-active.png">
            <img id="review-three" class="review-icon" @click="reviewThree()" src="../assets/carousel-inactive.png">
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        reviewOne() {
            document.getElementById('review').innerHTML =
            '<p class="review-text">“ Excellent work and outdid all expectations. It was enjoyable to work with them on a large important project and will be working with them again in the future.”</p><p class="author">Susan Jones</p>';
            document.getElementById('review-one').src = require("../assets/carousel-active.png");
            document.getElementById('review-two').src = require("../assets/carousel-inactive.png");
            document.getElementById('review-three').src = require("../assets/carousel-inactive.png");
        },   
        reviewTwo() {
            document.getElementById('review').innerHTML =
            '<p class="review-text">“ Outstanding job and exceeded all expectations. It was a pleasure to work with them on a sizeable first project and am looking forward to starting the next one asap.”</p><p class="author">Michael Hopkins</p>';
            document.getElementById('review-one').src = require("../assets/carousel-inactive.png");
            document.getElementById('review-two').src = require("../assets/carousel-active.png");
            document.getElementById('review-three').src = require("../assets/carousel-inactive.png");
        },
        reviewThree() {
            document.getElementById('review').innerHTML =
            '<p class="review-text">“ Fantastic work and surpassed all expectations. It was a joy to work with them on a substantial second project and we are looking forward to working together again.”</p><p class="author">John Smith</p>';
            document.getElementById('review-one').src = require("../assets/carousel-inactive.png");
            document.getElementById('review-two').src = require("../assets/carousel-inactive.png");
            document.getElementById('review-three').src = require("../assets/carousel-active.png");
        }

    }
}
</script>

<style lang="scss">

@import '../style/variables.scss';
@import '../style/_mixins.scss'; 
    
.review-icons > img {
    cursor: pointer;
}

.review-icon {
    padding: 50px 5px;
}

.review-text, .author {
    font-family: $headerFont;
    color: #ffffff;
    font-weight: bold;
}

.review-text {
    font-size: 23px;
    line-height: 35px;
    letter-spacing: 1px;
    padding: 75px 210px 0;
}
.author {
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 1px;   
}
 
.reviews {
    background-color: $themeColorBlue;
}

</style>