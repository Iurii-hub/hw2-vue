<template>
  <div>
      <!-- <h3>AddTodo</h3> -->
      <input type="text" v-model="todo">
      <button @click="add">Add</button>

  </div>
</template>


<script>

export default {
    name: "AddTodo",

    data () {
      return {
        todo: "",
      }
    },

    methods: {
      add() {
        this.$emit("add", this.todo)
      }
    }

}

</script>


<style>

</style>