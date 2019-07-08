<template>
<div id="process-video">
                <div id="video-video">
                    <a href="#">
                        <video @mouseout="hidePause()" :poster="videoPoster" id="video" @ended="showPlay()">
                            <source :src="videoLink" type="video/mp4">
                        </video>
                    </a>
                </div>
                <img id="play-button" @click="playVid()" src="../assets/play-button.png">
                <div><img id="pause-button" @click="pauseVid()" src="../assets/pause-button.png"></div>
            </div>
</template>

<script>
    export default {
        data() {
            return {
                videoLink: require("../assets/Maneki-Neko.mp4"),
                videoPoster: require("../assets/Maneki-Neko.jpg"),  
                }
            },
        methods: {
            playVid() {
                document.getElementById("play-button").style.visibility = "hidden";
                video.play();
                this.showPause();
                setTimeout(this.pauseEvent, 1000);
            },
            showPause() {
                document.getElementById("pause-button").style.visibility = "visible";
            },
            hidePause() {
                document.getElementById("pause-button").style.visibility = "hidden";
            },
            showPlay() {
                document.getElementById("play-button").style.visibility = "visible";
            },
            pauseVid() {
                video.pause();
                this.hidePause();
                document.getElementById("video").removeEventListener("mouseover", this.showPause);
                this.showPlay();
            },
            pauseEvent() {
                document.getElementById("video").addEventListener("mouseover", this.showPause);
            }
            
        }
    }

</script>

<style lang="scss">
@import '../style/variables.scss';
@import '../style/_mixins.scss'; 
    
#video {
    width: 90%;
    height: auto;
    text-align: center;
    padding-bottom: 50px;
}

#process-video {
    position: relative;
}

.process {
    padding: 25px;
}

#pause-button {
    visibility: hidden;
}
    
#play-button, #pause-button {
    @include centerIcons();
}   
</style>