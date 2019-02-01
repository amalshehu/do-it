<template>
  <div>
    <div v-bind:key="todo.id" v-for="todo in todos">
      <Todo v-bind:todo="todo"/>
    </div>
  </div>
</template>

<script>
import Todo from "./Todo";
export default {
  name: "Todos",
  components: { Todo },
  props: ["todos"]
};
</script>

<style scoped>
</style>
