<template>
<body>
  <div>
    <h1>LEONARDO DA VINCI RESTAURANTE</h1>
    <h1><nuxt-link to="./about">Menü</nuxt-link></h1>
    <h1><nuxt-link to="./contact">Kontaktseite</nuxt-link></h1>
    <img src="./leonardo.jpg" alt=""> 
    

    
    
  </div>
 
</body>
</template>

<script>
export default {
  name:"index" 
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

</style>