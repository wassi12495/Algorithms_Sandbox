<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <p>{{this.array}}</p>
    <Quicksort :array="this.array"/>
    <Mergesort :array="this.array"/>
  </div>
</template>

<script>
import Quicksort from "./components/Quicksort.vue";
import Mergesort from "./components/Mergesort.vue";
export default {
  name: "app",
  components: {
    Quicksort: Quicksort,
    Mergesort: Mergesort
  },
  data() {
    return {
      array: [8, 10, 4, 11, 3, 9]
    };
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
