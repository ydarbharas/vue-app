<template>
    <div class="header-text">
	   <h1> {{ title }}</h1>
        <p>{{ text }}</p>
        <button>Contact Us</button>
        </div>
</template>

<script>
export default {
    data() {
        return {
            title: "We Design and Develop",
            text: "We are a new design studio based in USA. We have over 20 years of combined experience, and know a thing or two about designing websites and mobile apps."
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss';   

.header-text {
    @include gridOctoColumns();
    clear: right;
    text-align: left;
    line-height: 1.5;
    padding: 100px;
    h1 {
        @include headerFontStyle();
        grid-column: 6 / 9; 
    }
    p {
        @include textFontStyle();
        grid-column: 6 / 9;
        padding-bottom: 30px;
    }
    button {
        @include buttonFormat();
        grid-column: 6 / 8;
    }
}
</style>

