<template>
  <span class="btn" @click="myFunc">{{text}}</span>
</template>

<script>
export default {
  setup() {},
  props: {
    text: String,
  },
};
</script>
