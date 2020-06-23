<template>
<body>
  <div>
    <h1>LEONARDO DA VINCI RESTAURANTE</h1>

    <table style="width:100%">
            <tr>
                <td><h1><nuxt-link to="/">Startseite </nuxt-link></h1></td>
                <td><h1><nuxt-link to="./contact">Kontaktseite</nuxt-link></h1></td>
                <td><h1><nuxt-link to="./Gästebuch">Gästebuchseite</nuxt-link></h1></td>
                <td><h1><nuxt-link to="./about">Menü</nuxt-link></h1></td>
                
            </tr>
        </table>
        <br>
        <br>

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
    
    background-color: brown;
   
  }

</style>