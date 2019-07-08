<template>
<div class="clients" >
    <div v-for="client in clientImageList">
        <img class="client-image" :src="client">
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            clientImageList: [require("../assets/1.png"), require("../assets/2.png"), require("../assets/3.png"), require("../assets/4.png"), require("../assets/5.png")]
        }
    }
}

</script>

<style lang="scss">
    
@import '../style/_mixins.scss'; 

.clients {
    height: 200px;
    @include flexCenter();
}
</style>