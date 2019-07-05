<template>
    <div>
        <img class="logo" src="./assets/logo.png">
        <ul class="nav">
            <li><a id="active" href="index.html">Home</a></li>
            <li><a class= "about" href="#about">About</a></li>
            <li><a class= "work" href="#work">Work</a></li>
            <li><a class= "process-" href="#process">Process</a></li>
            <li><a class= "services-" href="#services">Services</a></li>
            <li><a class= "testimonials-" href="#testimonials">Testimonals</a></li>
            <li><a class= "contact-" href="#contact">Contact</a></li>
            </ul>   
    </div>
</template>

<script>
</script>

<style>
.nav {
    float: right;
    margin: 0;
    padding: 10px;
}

.nav > li {                                                             
    display: inline-block;
    padding: 25px 9px 10px 9px;                               
} 

.nav > li > a:hover {
     color: #10c9c3;
 }

.nav > li a {                                               
     text-decoration: none;
     color: #191919;
     font-size: 14px;
     padding: 5px 0px 5px 0px
 }

.logo {
    float: left;
    padding: 35px 0px 0px 75px;
    height: auto;
}

li {
    text-transform: uppercase;
    font-weight: bold;
    letter-spacing: 1px;
}

#active {
    color: #10c9c3;
}
</style>

// Sarahs-iMac:Documents sarahbrady$ cd vue-app
// Sarahs-iMac:vue-app sarahbrady$ npm run serve