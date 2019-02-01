<template>
  <div>
    <p>Todo Item</p>
  </div>
</template>

<script>
export default {
  name: "Todo"
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
