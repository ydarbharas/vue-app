<template>
    <div>
        <div class="skills__info" v-for="skill in skills">
            <p class="skills__info__name">{{ skill.skillsName }}</p>
            <p class="skills__info__percentage">{{ skill.skillsPercentage }}</p>
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
                { id: 1, skillsName: "ui/ux design", skillsPercentage: "75%", skillsClass: "skills__info__design"},
                { id: 2, skillsName: "web development", skillsPercentage: "90%", skillsClass: "skills__info__web-dev"},
                { id: 3, skillsName: "marketing", skillsPercentage: "65%", skillsClass: "skills__info__marketing"}//,
// Add new skill test { id: 4, skillsName: "photography", skillsPercentage: "80%", skillsClass: "advertising"}
            ]            
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss';

.skills__info__name, .skills__info__percentage {
    display: inline;   
}

.skills__info__percentage {
    padding: 20px
}

#progress-bar-back {
    background-color: #d8d8d8;
    height: 5px;
    margin-bottom: 30px;
    margin-top: 15px
}

.skills__info {
    width: 50%;
    padding: 0px 50px;
    text-align: left;
    text-transform: uppercase;
    font-family: $textFont;
    font-size: 0.7em;
    letter-spacing: 1px;
    font-weight: bold;
}
 
.skills__info__design {
    @include skillsProgressBar();
    width: 75%;
}

.skills__info__web-dev {
    @include skillsProgressBar();
    width: 90%;
}
    
.skills__info__marketing {
    @include skillsProgressBar();
     width: 65%;
}

/* .photography {
    width: 80%;
    background-color: #10c9c3;
    height: 5px;
} */
</style>