<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Quicksort/>
  </div>
</template>

<script>
import Quicksort from "./components/Quicksort.vue";
export default {
  name: "app",
  components: {
    Quicksort: Quicksort
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
