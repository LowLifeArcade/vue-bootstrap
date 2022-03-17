<script setup>
import { defineProps } from 'vue';
const props = defineProps({
  message: String});
</script>
/**
<div>
// export default {
//   name: 'TaskComp',
//   props: {
//     task: Object,
//   },
//   data() {
//     return {
//       message: 'hi',
//     };
//   },
//   methods: {
//     day() {
//       this.message = this.message == 'hi' ? 'gotcha' : 'hi';
//     },
//   },
// };
// </div>

<template>
  <h3>{{ task.day }}</h3>
  <p role="button" @click="day">{{ props.message }}</p>
</template>

<style></style>
