<script>
import TheWelcome from "./TheWelcome.vue";

export default {
  data() {
    return {
      count: 1,
      classTitle: "title",
    };
  },
  methods: {
    increment() {
      this.count++;
    },
  },
};
</script>

<template>
  <h1 v-bind:class="classTitle">{{ count }}</h1>
  <p>vue로 확인하는 웹페이지입니다. 아래 버튼을 누르면 값이 1씩 증가합니다</p>
  <button v-on:click="increment">1+</button>
</template>

<style>
.title {
  color: red;
}
</style>
