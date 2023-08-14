<template>
  <div class="block_app">
      <div class="caption">Vue Todo App</div>
      <ul>
          <li v-bind:key="item.id" v-for="item in todoEntries">
              <ToDoItem v-bind:todoItem="item" />
          </li>   
      </ul>
      
  </div>
   
</template>

<script>
import ToDoItem from "./ToDoItem.vue";
export default {
  name: 'ToDos',
  components: {
      ToDoItem
  },
  props: [
    "todoEntries"
]
}
</script>


<style scoped src="../assets/css/style.css">
/* @import '../assets/css/style.css'; */
</style>