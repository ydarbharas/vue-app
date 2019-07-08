<template>
    <div class="header__text">
	   <h1> {{ title }}</h1>
        <p>{{ text }}</p>
        <button><a href=#contact>{{buttonText}}</a></button>
        </div>
</template>

<script>
export default {
    data() {
        return {
            title: "We Design and Develop",
            text: "We are a new design studio based in USA. We have over 20 years of combined experience, and know a thing or two about designing websites and mobile apps.",
            buttonText: "Contact Us"
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss';   

.header__text {
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
        a {
            text-decoration: none;
            color: $themeColorWhite;
        }
    }
}
</style>

