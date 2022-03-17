<template>
  <div :key="task.id" v-for="task in tasks">
    <task-comp :task="task" />
  </div>
</template>

<script>
import TaskComp from './TaskComp.vue';

export default {
  components: {
    TaskComp,
  },
  name: 'tasks-component',
  props: {
    tasks: Array,
  },
};
</script>
