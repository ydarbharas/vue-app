<template>
    <div id="skills">
        <h2>Professional Skills</h2>
        <ProfessionalSkillsBars class="design" skill-name="ui/ux design" skill-percentage="75%" />
        <ProfessionalSkillsBars class="web-dev" skill-name="web development" skill-percentage="90%" />
        <ProfessionalSkillsBars class="marketing" skill-name="marketing" skill-percentage="65%" />
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
#skills {
    background-size: contain;
    background-repeat: no-repeat;
    background-position: right;
    height: 640px;
    background-image: url(../assets/skills-background-image.jpg);
    background-color: #f3f6fb;  
}
    
    
.design #progress-bar-front {
    width: 75%;
    background-color: #10c9c3;
    height: 5px;
}

.web-dev #progress-bar-front {
    width: 90%;
    background-color: #10c9c3;
    height: 5px;
}
    
.marketing #progress-bar-front {
    width: 65%;
    background-color: #10c9c3;
    height: 5px;
}
</style>
