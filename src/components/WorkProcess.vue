<template>
<div>
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

<style>

</style>