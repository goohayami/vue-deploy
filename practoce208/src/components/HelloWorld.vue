<template>
  <h2><span>This is Vue.js lecture 75</span></h2>
  <div v-for="name in names" key="name">{{ name }}</div>

  <input type="text" v-model="ga">
  <p>{{ ga }}</p>
</template>

<script>
import { ref } from "vue";

export default {
  name: "Home",
  setup() {
    const names = ref(["mario", "luiji", "koopa"]);

    return { names };
  },
};
</script>

<style scoped>
span {
  color: red;
}
</style>
