<template>
    <div>
        <h1>LEONARDO DA VINCI RESTAURANTE</h1>
        <table style="width:100%">
            <tr>
                <td><h1><nuxt-link to="/">Startseite </nuxt-link></h1></td>
                <td><h1><nuxt-link to="./contact">Kontaktseite</nuxt-link></h1></td>
                <td><h1><nuxt-link to="./Gästebuch">Gästebuchseite</nuxt-link></h1></td>
                <td><h1>Menü</h1></td>
                
            </tr>
        </table>
    
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
td {
    width: 25%;
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