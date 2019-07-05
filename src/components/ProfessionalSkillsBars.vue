<template>
    <div>
        <p class="skill-name">{{ skillName }} {{ skillPercentage }}</p>
        <div id="progress-bar-back">
            <div class="progress-bar-front"></div>
        </div>
    </div>
</template>

<script>
export default {
    props: ["skillName", "skillPercentage"]
}
</script>

<style>
.skill-name {
    font-weight: bold;
    display: inline;
    padding-bottom: 50px;
}




#progress-bar-front {
    background-color: #10c9c3;
    height: 5px;
}

#progress-bar-back .design {
  width: 75%;
}

#progressbar-back .web-dev {
  width: 90%;
}

#progressbar-back .marketing {
  width: 65%;
}

.skills-info {
    width: 50%;
    padding: 170px 50px;
    text-align: left;
}

</style>