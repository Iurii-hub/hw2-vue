<template>
  <div>
      <!-- <h3>TodoItem</h3> -->
      <h4>{{todos}}</h4>

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

}


</script>


<style>

</style>

