<template>
    <div>
        <form>
            <input v-for="contact in contactForm" :class="contact.inputClass" :placeholder="contact.inputPlaceholder">
        </form>
        <button class="submit">{{sendMessageButton}}</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            contactForm: [
                {id: 1, inputClass: "form", inputPlaceholder: "Your Name"},
                {id: 2, inputClass: "form", inputPlaceholder: "Your Email"},
                {id: 3, inputClass: "form-input", inputPlaceholder: "Your Title"},
                {id: 4, inputClass: "form-input-large", inputPlaceholder: "Your Comment"}
            ],
            sendMessageButton: "Send Message"
        }
    }    
}
</script>

<style lang="scss">

@import '../style/variables.scss';
@import '../style/_mixins.scss'; 

.form-input, .form-input-large {
    width: 50%;
    padding: 10px;
    margin: 10px;
}

.form-input-large {
    height: 100px;
}

input {
    border: 0;
}

.form {
    width: 30.5em;
    padding: 10px;
    margin: 10px;
    @include textFontStyle();
    
}
    
.submit {
        @include buttonFormat();
}
    
</style>