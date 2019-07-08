<template>
    <div class="testimonials">
        <a name="testimonials"></a>
        <div id="testimonials">
            <p class="testimonials__text">“ Outstanding job and exceeded all expectations. It was a pleasure to work with them on a sizeable first project and am looking forward to starting the next one asap.”</p>
            <p class="testimonials__author">Michael Hopkins</p>
        </div>
        <div class="testimonials__alt">
            <img id="testimonials__alt__one" class="testimonials__alt__icon" @click="reviewOne()" src="../assets/carousel-inactive.png">
            <img id="testimonials__alt__two" class="testimonials__alt__icon" @click="reviewTwo()" src="../assets/carousel-active.png">
            <img id="testimonials__alt__three" class="testimonials__alt__icon" @click="reviewThree()" src="../assets/carousel-inactive.png">
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        reviewOne() {
            document.getElementById('testimonials').innerHTML =
            '<p class="testimonials__text">“ Excellent work and outdid all expectations. It was enjoyable to work with them on a large important project and will be working with them again in the future.”</p><p class="testimonials__author">Susan Jones</p>';
            document.getElementById('testimonials__alt__one').src = require("../assets/carousel-active.png");
            document.getElementById('testimonials__alt__two').src = require("../assets/carousel-inactive.png");
            document.getElementById('testimonials__alt__three').src = require("../assets/carousel-inactive.png");
        },   
        reviewTwo() {
            document.getElementById('testimonials').innerHTML =
            '<p class="testimonials__text">“ Outstanding job and exceeded all expectations. It was a pleasure to work with them on a sizeable first project and am looking forward to starting the next one asap.”</p><p class="testimonials__author">Michael Hopkins</p>';
            document.getElementById('testimonials__alt__one').src = require("../assets/carousel-inactive.png");
            document.getElementById('testimonials__alt__two').src = require("../assets/carousel-active.png");
            document.getElementById('testimonials__alt__three').src = require("../assets/carousel-inactive.png");
        },
        reviewThree() {
            document.getElementById('testimonials').innerHTML =
            '<p class="testimonials__text">“ Fantastic work and surpassed all expectations. It was a joy to work with them on a substantial second project and we are looking forward to working together again.”</p><p class="testimonials__author">John Smith</p>';
            document.getElementById('testimonials__alt__one').src = require("../assets/carousel-inactive.png");
            document.getElementById('testimonials__alt__two').src = require("../assets/carousel-inactive.png");
            document.getElementById('testimonials__alt__three').src = require("../assets/carousel-active.png");
        }

    }
}
</script>

<style lang="scss">

@import '../style/variables.scss'; 
    
.testimonials {
    background-color: $themeColorBlue;
}

.testimonials__text, .testimonials__author {
    font-family: $headerFont;
    color: $themeColorWhite;
    font-weight: bold;
}

.testimonials__text {
    font-size: 23px;
    line-height: 35px;
    letter-spacing: 1px;
    padding: 75px 210px 0;
}
.testimonials__author {
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 1px;   
}

.testimonials__alt__icon {
    padding: 50px 5px;
    cursor: pointer;
}


</style>