<template>
    <div>
        <img class="logo" src="../assets/logo.png">
        <ul class="nav">
            <li><a id="active" href="index.html">Home</a></li>
            <li><a class= "nav__about" href="#about">About</a></li>
            <li><a class= "nav__work" href="#work">Work</a></li>
            <li><a class= "nav__process" href="#process">Process</a></li>
            <li><a class= "nav__services" href="#services">Services</a></li>
            <li><a class= "nav__testimonials" href="#testimonials">Testimonals</a></li>
            <li><a class= "nav__contact" href="#contact">Contact</a></li>
        </ul>   
    </div>
</template>

<script>
   

</script>

<style lang="scss">
@import '../style/variables.scss';

.nav {
    float: right;
    margin: 0;
    padding: 10px;
    font-family: $textFont;
    li {
        display: inline-block;
        padding: 25px 9px 10px 9px; 
        text-transform: uppercase;
        font-weight: bold;
        letter-spacing: 1px; 
    }
    li a {
        text-decoration: none;
        color: #191919;
        font-size: 14px;
        padding: 5px 0px 5px 0px;
        &:hover {
        color: #10c9c3; 
        }
    }
}

.logo {
    float: left;
    padding: 35px 0px 0px 75px;
    height: auto;
}

#active {
    color: $themeColorBlue;
}
    
</style>

