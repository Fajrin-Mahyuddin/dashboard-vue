<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import TestedComponent from './components/TestedComponent.vue';
const test = "blabla"
const propsFromParents = "this a props from parents"
const clickData = () => {
  console.log("this is at the parents");
}
</script>

<template>
  <div>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld :msg=test />
  <TestedComponent :title=propsFromParents :fun="clickData" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
