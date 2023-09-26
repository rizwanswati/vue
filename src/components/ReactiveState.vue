<script setup>
import {ref} from "vue";
var count = ref(0);
console.log(count)
console.log(count.value)

function increment() {
  count.value++
}


</script>

<template>
  <div>Simple</div>
  <button @click="count++">count</button>
  <div>{{count}}</div>

  <div>complex</div>
  <button @click="increment">increment</button>
  <div>{{count}}</div>
</template>

<style scoped>

</style>