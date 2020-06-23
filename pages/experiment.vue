<template>

    <div id="todo-list-example">
        
      <table style="width:100%">
            <tr>
                <td><h1><nuxt-link to="/">Startseite </nuxt-link></h1></td>
                <td><h1><nuxt-link to="./contact">Kontaktseite</nuxt-link></h1></td>
                <td><h1>Gästebuchseite</h1></td>
                <td><h1><nuxt-link to="./about">Menü</nuxt-link></h1></td>
                
            </tr>
        </table>     



            <label for="new-todo">Add a todo</label>
            <input
                v-model="newTodoText"
                id="new-todo"
                placeholder="E.g. Feed the cat"
                >
            <button v-on:click="addtodo" >Add</button>

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
{{newTodoText}}
    <div v-for="listItem in list">
        {{listItem.name}}
        {{listItem.msg}}
        {{listItem.place}}
<hr>

    </div>
    </div>
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
            this.list.push({name:"Nachricht von", place:" " + this.newTodoText})

            
        } 
    }
}


</script>

