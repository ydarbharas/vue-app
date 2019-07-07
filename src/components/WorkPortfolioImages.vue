<template>
<div class="container">
   <div v-for="image in images" :class="image.imageClass" class="image-container">
                <img :src="image.imageLink" class="image">
                <div class="overlay">
                    <div class="hover-icon"><img src="../assets/pe-7s-look.png"></div>
                </div>
            </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            images: [
                {id: 1, imageLink: require("../assets/portfolio-1.jpg"), imageClass: "column-1 row-1"},
                {id: 2, imageLink: require("../assets/portfolio-2.jpg"), imageClass: "column-2 row-2"},
                {id: 3, imageLink: require("../assets/portfolio-3.jpg"), imageClass: "column-3 row-1"},
                {id: 4, imageLink: require("../assets/portfolio-4.jpg"), imageClass: "column-4 row-2"},
                {id: 5, imageLink: require("../assets/portfolio-5.png"), imageClass: "column-1 row-1"},
                {id: 6, imageLink: require("../assets/portfolio-6.jpg"), imageClass: "column-2 row-2"},
                {id: 7, imageLink: require("../assets/portfolio-7.jpg"), imageClass: "column-3 row-1"},
                {id: 8, imageLink: require("../assets/portfolio-8.jpg"), imageClass: "column-4 row-2"}
            ]
        }
    }
}

</script>

<style>
    
.image-container {
  position: relative;
}

    
.image {
    width: 100%
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 98.9%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background-color: black;
}

.image-container:hover .overlay {
  opacity: 0.7;
}


.row-1 {
    margin-bottom: -23px;
}

.row-2 {
    margin-bottom: -31px;
}
    
    .column-1 {
    grid-column: 1 / 3;
}

.column-2 {
    grid-column: 3 / 5;
}

.column-3 {
    grid-column: 5 / 7;
}

.column-4 {
    grid-column: 7 / 9;
}
    
.container {
    display: grid;
    grid-template-columns: repeat(8, 1fr);
    grid-template-rows: auto;
    text-align: center;
    grid-row-gap: 15px;
    margin: 0px;
    
    }
    
.hover-icon {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  cursor: pointer;
}   
</style>