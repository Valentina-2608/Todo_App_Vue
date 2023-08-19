<template>
  <div class="block_app">
      <div class="caption">Vue Todo App</div>
      <div class="tasks">
          <div v-bind:key="item.id" v-for="item in todoEntries" class="todo_item">
          <div class="todo_title">
            <ToDoItem v-bind:todoItem="item" />
          </div>
            <button class="delete_todo">Delete todo</button>
            <button class="check_todo">Check todo</button>
          </div>   
      </div>
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