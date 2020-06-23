<template>
<body>
    <h1>LEONARDO DA VINCI RESTAURANTE</h1>
    <div id="todo-list-example">
        
      <table style="width:100%">
            <tr>
                <td><h1><nuxt-link to="/">Startseite </nuxt-link></h1></td>
                <td><h1><nuxt-link to="./contact">Kontaktseite</nuxt-link></h1></td>
                <td><h1>Gästebuchseite</h1></td>
                <td><h1><nuxt-link to="./about">Menü</nuxt-link></h1></td>
                
            </tr>
        </table>     


<br>
            <label style="font-Size:25px" for="new-todo">Name</label>
            <input
            style="font-Size:25px"
                v-model="newTodoText"
                id="new-todo"
                placeholder="Nachricht eintragen"
                >
            <button style="font-Size:25px" v-on:click="addtodo" >Hinzugügen</button>

        <ul>
            <li
                is="todo-item"
                v-for="(todo, index) in todos"
                v-bind:key="todo.id"
                v-bind:title="todo.little"
                v-on:remove="todos.splice(index, 1)"
            ></li>
        </ul>
        
{{count}}

    <div v-for="listItem in list">
        {{listItem.name}}
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
           newTodoText:''
    
        }
    },
    methods:{
        addtodo()  {
            this.count = this.count + 1;
            this.list.push({name:"Danke für Ihren Besuch", place:" " + this.newTodoText})

            
        } 
    }
}
</script>

