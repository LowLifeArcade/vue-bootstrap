<template>
  <div :key="task.id" v-for="task in tasks">
    <h3>{{ task.day }}</h3>
  </div>
</template>

<script>
export default {
  name: 'tasks-component',
  props: {
    tasks: Array,
  },
};
</script>
