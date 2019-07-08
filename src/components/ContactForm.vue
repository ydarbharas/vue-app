<template>
<div class="contact">
    <div>
                <a name="contact"></a>
                <h2>{{ contactForm.title }}</h2>
                <p class="contact__info"> {{ contactForm.text }}</p>
            </div>
            <div>
                <ContactFormInput/>
            </div>
    </div>           
</template>

<script>
import ContactFormInput from './ContactFormInput.vue'

export default {
    data() {
        return {
            contactForm: {
                title: "Need a Project?",
                text: "Let us know what you're looking for in an agency. We'll take a look and see if this could be the start of something beautiful."
            }
        }
    },
    components: {
        ContactFormInput
    }
}
</script>

<style lang="scss">

@import '../style/variables.scss';
@import '../style/_mixins.scss'; 

.contact {
    background-color: $themeColorGrey;
    padding: 50px 0px;
    h2 {
        @include headerFontStyle();
    }
    p {
        @include textFontStyle();
        padding: 0 360px;
    }
}

</style>