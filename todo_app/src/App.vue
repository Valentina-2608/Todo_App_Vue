<template>
  <div id="app">
    <ToDos v-bind:todoEntries="todoEntries"/>
  </div>
</template>

<script>

import ToDos from './components/ToDos.vue'

export default {
  name: 'App',
  components: {
    ToDos
  },
  data(){
    return {
      todoEntries: [
        {id:1,
        title:'Go shopping',
        completed:false
        },
        {id:2,
        title:'Clean flat',
        completed:false
        },
        {id:3,
        title:'Wash up',
        completed:false
        }

      ]

    }
  }
}
</script>



<style scoped src="./assets/css/style.css">
/* @import 'assets/css/style.css'; */
</style>