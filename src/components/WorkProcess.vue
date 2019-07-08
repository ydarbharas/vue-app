<template>
<div class="process">
    <a name="process"></a>
    <h2>{{ title }}</h2>
    <p>{{ text }} </p>
    <WorkProcessVideo/>
</div>
</template>

<script>
import WorkProcessVideo from './WorkProcessVideo.vue'
export default {
    components: {
            WorkProcessVideo
    },
    data() {
        return {
            title: "Our Work Process",
            text: "Was years it seasons was there form he in in them together over that third sixth gathered female creeping bearing behold years."
        }
    }
    
}
</script>

<style lang="scss">
    
@import '../style/_mixins.scss'; 

.process {
    h2 {
        @include headerFontStyle();
        padding-top: 100px;
    }
    p {
        @include textFontStyle();
        padding: 0 300px 50px 300px;
    }   
}
</style>