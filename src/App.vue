<template>
  <TodoItem/>
  <TodoList/>
</template>

<script>
import TodoList from './components/TodoList.vue'
import TodoItem from './components/TodoItem.vue'

export default {
  name: 'App',
  components: {
    TodoList,
    TodoItem
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

body {
  background-color: grey;
}

button {
  height: 18px;
  outline: 1px solid ;
  color: gray;
}
</style>
