<template>
    <div>
    <h1 class="menu">Menü</h1>
    <h1><nuxt-link to="/">Startseite </nuxt-link></h1>
    <h1><nuxt-link to="./contact">Kontaktseite</nuxt-link></h1>
    <img src="./pizza.jpg" alt="Pizza Margherita" >
    <h2>Pizza Magherita 15 Euro</h2>
    <hr>
    <img src="./pasta.jpg" alt="Italien Pasta">
    <h2>Pasta de Italia 12 Euro</h2> 
    <hr>
    <img src="./crep.jpg" alt="Crepe">
    <h2>Crepe 9 Euro</h2>

    
    </div>
</template>

<script>
export default {
    name:"about"
}
</script>
<style scoped>

body {
    background-color: burlywood;
    text-align: center;
  }
  h1 {
    font-family: initial;
    border: 15px solid brown;
    background-color: brown;
    margin-block: 15px;
  }
.menu{
        color:black;
    }

img{
width: 500px; 
height: 400px;
    }
h1{
     font-family: initial;
}

h2{
     font-family: initial;

}
</style>