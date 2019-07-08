<template>
    <div>
        <img class="logo" src="../assets/logo.png">
        <ul class="nav">
            <li v-for="nav in navBar"><a :id="nav.navId" :class="nav.navClass" :href="nav.navLink">{{nav.navName}}</a></li>
        </ul>   
    </div>
</template>

<script>
   export default {
       data() {
           return {
               navBar: [
                   {id: 1, navName: "Home", navClass: "nav__home", navLink: "index.html", navId: "active", },
                   {id: 2, navName: "About", navClass: "nav__about", navLink: "#about", navId: ""},
                   {id: 3, navName: "Work", navClass: "nav__work", navLink: "#work", navId: ""},
                   {id: 4, navName: "Process", navClass: "nav__process", navLink: "#process", navId: ""},
                   {id: 5, navName: "Services", navClass: "nav__services", navLink: "#services", navId: ""},
                   {id: 6, navName: "Testimonials", navClass: "nav__testimonials", navLink: "#testimonials", navId: ""},
                   {id: 7, navName: "Contact", navClass: "nav__contact", navLink: "#contact", navId: ""},
               ]
           }
       }
   }
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
