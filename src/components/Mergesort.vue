<template>
  <div class="merge">
    <p>Merge Sort: {{mergeSort(this.array)}}</p>
  </div>
</template>

<script>
import { log } from "util";
export default {
  name: "MergeSort",
  props: ["array"],
  data() {
    return {};
  },
  methods: {
    merge(left, right) {
      // console.log("Merge", left, right);
      let result = [];
      let i = 0;
      let j = 0;
      let k = 0;
      while (i < left.length && j < right.length) {
        if (left[i] <= right[j]) {
          result.push(left[i]);
          console.log("Left added ", result);
          i++;
        } else {
          result.push(right[j]);
          console.log("right added ", result);
          j++;
        }
        k++;
      }

      console.log("result", result);
      return result.concat(left.slice(i)).concat(right.slice(j));
    },
    mergeSort(a) {
      console.log("MergeSort", a);
      if (a.length === 1) {
        return a;
      }
      const q = Math.floor(a.length / 2);

      const left = a.slice(0, q);
      const right = a.slice(q);
      console.log("Left split", left);
      console.log("right split", right);
      // let x = this.mergeSort(left);
      // let y = this.mergeSort(right);
      // let z = this.merge(x, y);
      // console.log("x", x, "y", y, "z", z);

      return this.merge(this.mergeSort(left), this.mergeSort(right));
    }
  }
};
</script>

<style>
</style>
