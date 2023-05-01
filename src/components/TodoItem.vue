<template>
  <h1>Task Tracker</h1>
    <div class="todos">
      <input type="text" v-model="todo" placeholder="Add a Todo to Track!">
      <button @click="addTodo">Add Todo</button>
      <ul>
        <li v-for="todo in todos" v-bind:key="todo">
          <input type="checkbox">
          <label for="checkbox">{{ todo }}</label>
        </li>

      </ul>
    </div>
  </template>
  
  <script>
  export default {
    name: 'TodoItem',
    props: {
     
    },
    data() {
      return {
        todos: [
          "Make breakfast",
          "Take a Shower",
          "Go to the Store"
        ],
        todo: ""
      }
    },
    methods: {
      addTodo() {
        this.todos.push(this.todo)
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }

  input {
    height: 18px;
  }

  button {
    height: 18px;
  }

  .todos {
  display: block;
  padding: 10px;
  margin: auto;
  width: 10%;
}
  </style>