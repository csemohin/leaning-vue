<template>
  <div id="app">
    <div class="container">
      <Todos :todos="todos" />
    </div>
  </div>
</template>

<style lang="scss"></style>

<script>
import Todos from "@/components/Todos";
export default {
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          item: "Item one",
          completed: true
        },
        {
          id: 2,
          item: "Item two",
          completed: false
        },
        {
          id: 3,
          item: "Item three",
          completed: true
        }
      ]
    };
  }
};
</script>
