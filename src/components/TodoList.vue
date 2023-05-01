<template>
  <div></div>
</template>

<script>
import TodoItem from './TodoItem.vue';

import (TodoItem)
export default {
  name: 'TodoList',
  props: {
    msg: String
  },
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

.container {
  display: flex;
  text-align: center;
  padding: 10px;
  margin: auto;
  width: 10%;
}
</style>
