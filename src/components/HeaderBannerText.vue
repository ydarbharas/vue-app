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
    clear: right;
    text-align: left;
    line-height: 1.5;
    padding: 50px 50px 90px 70px;
    @include gridOctoColumns();
}
    
.header-text > h1 {
    grid-column: 6 / 9;
}
    
.header-text > p {
    grid-column: 6 / 9;
}
    
.header-text > button {
    grid-column: 6 / 7;
    width: 50%;
}
    

</style>

