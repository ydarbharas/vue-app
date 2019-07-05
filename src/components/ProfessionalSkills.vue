<template>
    <div class="skills">
        <ProfessionalSkillsBars class="design" skillName="ui/ux design" skillPercentage="75%" />
        <ProfessionalSkillsBars class="web-dev" skillName="web development" skillPercentage="90%" />
        <ProfessionalSkillsBars class="marketing" skillName="marketing" skillPercentage="65%" />
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

<style>
    .skills {
    background-size: contain;
    background-repeat: no-repeat;
    background-position: right;
    height: 640px;
    background-image: url(../assets/skills-background-image.jpg);
    background-color: #f3f6fb;  
}
    
    #progress-bar-back {
    background-color: #d8d8d8;
    height: 5px;
    margin-bottom: 30px;
    margin-top: 15px
}
    
#progress-bar-front {
    background-color: #10c9c3;
    height: 5px;
}

#progress-bar-back.design {
  width: 75%;
}

#progressbar-back.web-dev {
  width: 90%;
}

