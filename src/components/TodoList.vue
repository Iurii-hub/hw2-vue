<template>
  <div>
      <div
      v-for="(to_do, i) in todo"
      :key="i"
      >

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
        }
    },

    components: {
        TodoItem
    },

    data () {
        return {

        }
    }
}

</script>


<style>

</style>