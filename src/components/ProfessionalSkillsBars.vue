<template>
    <div>
        <div class="skills-info">
            <p class="skill-name">{{ skillName }}</p>
            <p class="skill-percentage">{{ skillPercentage }}</p>
            <div id="progress-bar-back">
                <div id="progress-bar-front"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ["skill-name", "skill-percentage"]
}
</script>

<style>
    
.skill-name, .skill-percentage {
    font-weight: bold;
    display: inline;
    padding-bottom: 50px;
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
}

</style>