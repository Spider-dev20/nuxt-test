<template>
<body>
    <h1>LEONARDO DA VINCI RESTAURANTE</h1>
    <div>
        
      <table style="width:100%">
            <tr>
                <td><h1><nuxt-link to="/">Startseite </nuxt-link></h1></td>
                <td><h1><nuxt-link to="./contact">Kontaktseite</nuxt-link></h1></td>
                <td><h1>Gästebuchseite</h1></td>
                <td><h1><nuxt-link to="./about">Menü</nuxt-link></h1></td>
                
            </tr>
        </table>     

 
<br>
            <label style="font-Size:25px" for="new-name"></label>
            
            
            <input
            style="font-Size:25px"
                v-model="name_of_user"
                id="new-name"
                placeholder="Name"
                ><br>
            <input
            placeholder="Nachricht"
            v-model="msg_of_user"
            style="font-Size:25px">  <br><br>
            <button style="font-Size:25px" v-on:click="addname" >Hinzugügen</button>
            
            
            
         {{count}}   


        <ul>
            <li
                is="name-item"
                v-for="(name, index) in names"
                v-bind:key="name.id"
                v-bind:title="name.little"
                v-on:remove="name.splice(index, 1)"
            ></li>
        </ul>
        


    <div v-for="listItem in list">
        {{listItem.uname}}
        {{listItem.msg}}
        {{listItem.place}}
<hr>
<br>
   </div>
</div>
</body>                   
</template>

<script>
export default {
    data(){
        return {
            count:0,
            list: [],
           name_of_user:'',
           msg_of_user:''
    
        }
    },
    methods:{
        addname()  {
            this.count = this.count + 1;
            this.list.push({ uname:"" + this.name_of_user, place:": " + this.msg_of_user})
            
        } 
    }
}
</script>