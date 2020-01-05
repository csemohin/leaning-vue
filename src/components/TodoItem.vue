<template>
  <div>
    <p class="clear-fix" :class="[todoItem.completed ? 'is-completed']">
      <input type="checkbox" />
      {{ todoItem.item }}
      <button class="btn btn-sm btn-danger float-right">x</button>
    </p>
  </div>
</template>

<script>
export default {
  props: ["todoItem"]
};
</script>

<style lang="scss" scoped>
p {
  margin-bottom: 0;
}
p.is-completed {
  text-decoration: line-through;
}
</style>
