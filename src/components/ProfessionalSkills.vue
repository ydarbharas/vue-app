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

<style>
    
#skills {
    background-size: contain;
    background-repeat: no-repeat;
    background-position: right;
    height: 640px;
    background-image: url(../assets/skills-background-image.jpg);
    background-color: #f3f6fb;  
}
    
</style>
