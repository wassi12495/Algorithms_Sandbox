<template>
  <div id="quicksort">
    <h1>quicsort</h1>
    <p>{{quicksort(this.array)}}</p>
  </div>
</template>

<script>
export default {
  name: "Quicksort",
  data() {
    return {
      greeting: "Hello",
      array: [8, 10, 4, 11, 3]
    };
  },
  methods: {
    partition(a, p, r) {},
    quicksort(a) {
      let p = a[0];
      let r = a[a.length - 1];
      if (p < r) {
        console.log("here");
      }
    }
  }
};
</script>

<style>
</style>
