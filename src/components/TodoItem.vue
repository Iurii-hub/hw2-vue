<template>
  <div>
      <!-- <h3>TodoItem</h3> -->
      <h4>{{todos}}</h4>
      <button @click="remove">Delete</button>

  </div>
</template>


<script>
export default {
    name: "TodoItem",

    props: {
        todos: {
            type: String,
            required: true,
        }
    },

    methods: {
        remove() {
            this.$emit("remove", this.todo)
        }
    }
}


</script>


<style>

</style>

