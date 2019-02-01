<template>
  <div>
    <div v-bind:key="todo.id" v-for="todo in todos">
      <h2>{{todo.title}}</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: "Todos",
  props: ["todos"]
};
</script>

<style scoped>
</style>
