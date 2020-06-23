<template>

<body>
<h1>LEONARDO DA VINCI RESTAURANTE</h1>
  <div>

    <table style="width:100%">
            <tr>
                <td><h1><nuxt-link to="/">Startseite </nuxt-link></h1></td>
                <td><h1>Kontaktseite</h1></td>
                <td><h1><nuxt-link to="./Gästebuch">Gästebuchseite</nuxt-link></h1></td>
                <td><h1><nuxt-link to="./about">Menü</nuxt-link></h1></td>
                
            </tr>
        </table>

    <h2>Reservierung unter:</h2>
    <h3>0157353057</h3>
    <br>
    <hr>
    <h2>Adresse:</h2>
    <h3>Calle de Humbre 25</h3>
    <br>
    <hr>
    <h2>Öffnungszeiten</h2>
    <h3>Täglich von 11:00 bis 23:00 Uhr geöffnet</h3>
    <br>
    <hr>
    <h2>Email:</h2>
    <h3>veni.vici@gmx.de</h3>
    <br>
    <hr>
    <br>
    <img src="./restaurant.jpg" alt="">


    

    
  </div>

</body>

</template>

<script scoped>
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
  h2{
    margin-block: 15px;  
  }
  a {
    color: black;
  }
</style>