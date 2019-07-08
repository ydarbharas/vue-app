<template>
<div class="work-process">
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
    @import '../style/variables.scss';
    @import '../style/_mixins.scss'; 

.work-process {
    h2 {
        @include headerFontStyle();
        padding-top: 50px;
    }
    p {
        @include textFontStyle();
        padding-bottom: 30px;
    }   
}
</style>