<template>
    <div class="header-text">
	   <h1> We Design and Develop</h1>
        <p>We are a new design studio based in USA. We have over 20 years of combined experience, and know a thing or two about designing websites and mobile apps.</p>
        <button>Contact Us</button>
        </div>
</template>

<script>

</script>

<style>
    
.header-text {
    clear: right;
    text-align: left;
    line-height: 1.5;
    padding: 50px 50px 90px 70px;
    display: grid;
    grid-template-columns: repeat(8, 1fr);
    grid-template-rows: auto;
    grid-row-gap: 15px;
    margin: 0px;
}
    
.header-text > h1 {
    grid-column: 6 / 9;
}
    
.header-text > p {
    grid-column: 6 / 9;
}
    
.header-text > button {
    grid-column: 6 / 7;
    width: 50%;
}
    

</style>

