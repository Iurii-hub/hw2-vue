<template>
  <div>
      <!-- <h3>TodoList</h3> -->
      
      <div v-for="(todos, i) in todo" :key="i">
          <TodoItem :todos="todos" @remove = "remove"/>
      </div>

  </div>
</template>


<script>

import TodoItem from "@/components/TodoItem";

export default {
    name: "TodoList",

    props: {
        todo: {
            type: Array,
            // required: true,
        }
    },

    components: {
        TodoItem
    },

    methods: {
        remove(event) {
            this.$emit("remove", event)
        }
    }
}

</script>


<style>

</style>