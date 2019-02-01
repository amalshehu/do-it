<template>
  <div id="app">
    <Todos/>
  </div>
</template>

<script>
import Todos from "./components/Todos.vue";

export default {
  name: "app",
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        { id: 1, title: "Setup vue cli", done: true },
        { id: 2, title: "App scaffholding", done: true },
        { id: 3, title: "Component generation", done: false }
      ]
    };
  }
};
</script>
 
<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  line-height: 1.5;
}
</style>
