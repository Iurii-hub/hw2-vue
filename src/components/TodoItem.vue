<template>
  <div>
      <h5>{{to_do.action}}</h5>
      <p>{{to_do.status}}</p>

  </div>
</template>


<script>
export default {
    name: "TodoItem",

    props: {
        to_do: {
            type: Object,
        }
    },

    data () {
        return {
            dataPropsTodo: this.to_do
        }
    }
}


</script>


<style>

</style>