<template>
    <div>
        <div class="skills-info" v-for="skill in skills">
            <p class="skill-name">{{ skill.skillsName }}</p>
            <p class="skill-percentage">{{ skill.skillsPercentage }}</p>
            <div id="progress-bar-back">
                <div :class="skill.skillsClass"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            skills: [
                { id: 1, skillsName: "ui/ux design", skillsPercentage: "75%", skillsClass: "design"},
                { id: 2, skillsName: "web development", skillsPercentage: "90%", skillsClass: "web-dev"},
                { id: 3, skillsName: "marketing", skillsPercentage: "65%", skillsClass: "marketing"}//,
// Add new skill test { id: 4, skillsName: "photography", skillsPercentage: "80%", skillsClass: "advertising"}
            ]            
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss';

.skill-name, .skill-percentage {
    display: inline;   
}

.skill-percentage {
    padding: 20px
}

#progress-bar-back {
    background-color: #d8d8d8;
    height: 5px;
    margin-bottom: 30px;
    margin-top: 15px
}

.skills-info {
    width: 50%;
    padding: 0px 50px;
    text-align: left;
    text-transform: uppercase;
    font-family: $textFont;
    font-size: 0.7em;
    letter-spacing: 1px;
    font-weight: bold;
}
 
.design {
    @include skillsProgressBar();
    width: 75%;
}

.web-dev {
    @include skillsProgressBar();
    width: 90%;
}
    
.marketing {
    @include skillsProgressBar();
     width: 65%;
}

/* .photography {
    width: 80%;
    background-color: #10c9c3;
    height: 5px;
} */
</style>