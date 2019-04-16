<template>
  <div id="quicksort">
    <p>QuickSort: {{quicksort(this.array)}}</p>
  </div>
</template>

<script>
export default {
  name: "Quicksort",
  props: ["array"],
  data() {
    return {
      greeting: "Hello"
    };
  },
  methods: {
    partition(a, p, r) {},
    quicksort(a) {
      let p = a[0];
      let r = a[a.length - 1];
      console.log("p", p, "r", r);
      if (p < r) {
      }
    }
  }
};
</script>

<style>
</style>
