<template>
  <div class="todo-item" v-bind:class="{'is-complete': todo.done}">
    <p>
      <input type="checkbox" v-on:change="markComplete">
      {{todo.title}}
      <button class="del" @click="$emit('del-todo', todo.id)">x</button>
    </p>
  </div>
</template>

<script>
export default {
  name: "Todo",
  props: ["todo"],
  methods: {
    markComplete() {
      this.todo.done = !this.todo.done;
    }
  }
};
</script>

<style scoped>
.todo-item {
  background: floralwhite;
  padding: 10px;
  border-bottom: 1px #dddddd dotted;
}
.is-complete {
  text-decoration-line: line-through;
}
.del {
  background: red;
  color: #dddddd;
  border: none;
  padding: 5px 9px;
  border-radius: 50%;
  cursor: pointer;
  float: right;
}
</style>
