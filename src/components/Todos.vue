<template>
  <div>
    <div class="todos mt-3">
      <ul class="list-group">
        <li class="list-group-item" v-for="todo in todos" :key="todo.id">
          <TodoItem :todoItem="todo"/>
          
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import TodoItem from '@/components/TodoItem'
export default {
  components:{
    TodoItem
  },
  props: ["todos"]
};
</script>

<style lang="scss" scoped></style>
