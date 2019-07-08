<template>
    <div class="contact__form">
        <form>
            <input class="contact__form--small" placeholder="Your Name">
            <input class="contact__form--small" placeholder="Your Email"><br>
            <input class="contact__form--normal" placeholder="Your Title"><br>
            <input class="contact__form--large" id="comment" placeholder="Your Comment">
        </form>
        <button class="contact__form__submit">{{sendMessageButton}}</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            sendMessageButton: "Send Message"
        }
    }    
}
</script>

<style lang="scss">

@import '../style/variables.scss';
@import '../style/_mixins.scss'; 

input {
    border: 0;
}
    
.contact__form--normal, .contact__form--large {
    width: 51%;
    padding: 10px;
    margin: 10px;
    
}

.contact__form--large {
    height: 100px;
}

.contact__form--small {
    width: 25%;
    padding: 10px;
    margin: 10px;
    @include textFontStyle();
    
}
    
.contact__form__submit {
    @include buttonFormat();
}
    
</style>