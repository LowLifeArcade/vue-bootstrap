<script setup>
import { defineProps } from 'vue';
const props = defineProps({
  task: Object,
});

let message = 'hi';

function day() {
  message = message == 'hi' ? 'gotcha' : 'hi';
  console.log()
}

/**
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
*/
</script>

<template>
  <h3>{{ props.task.day }}</h3>
  <p role="button" @click="day" v-if="message">{{ message }}</p>
</template>

<style></style>
