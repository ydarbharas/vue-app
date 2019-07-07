<template>
    <div id="skills">
        <h2>Professional Skills</h2>
        <ProfessionalSkillsBars/>
    </div>
</template>

<script>
import ProfessionalSkillsBars from './ProfessionalSkillsBars.vue'
    
export default {
    components: {
        ProfessionalSkillsBars
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss'; 
    
#skills {
    background-size: contain;
    background-repeat: no-repeat;
    background-position: right;
    height: 640px;
    background-image: url(../assets/skills-background-image.jpg);
    background-color: #f3f6fb;
    h2 {
        @include headerFontStyle();
        text-align: left;
        padding: 200px 0px 10px 50px;
    }
}
    
</style>
