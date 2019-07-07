<template>
    <div class="about-us">
        <a name="about"></a>
            <div class="about-text">
                <h2>About Us</h2>
                <p>{{ text }}</p>
                <img :src="image">
                </div>
            </div>
</template>

<script>
export default {
    data() {
        return {
            text: "Divide have don't man wherein air fourth. Own itself make have night won't make. A you under seed appear which good give. Own give air without fowl moveth dry first heaven fruit, dominion she'd won't very all.",
            image: require("../assets/signature.png"),
        }
    }
}

</script>

<style lang="scss">
    
.about-text {
    padding: 60px 300px;
    h2 {
        font-size: 1.8em;
    }
    p {
    padding: 10px 0 20px 0;
    line-height: 1.5;    
    }
}
</style>