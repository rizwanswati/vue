<script setup>
  defineProps({
    msg:{
      required:true,
      type:String
    }
  })
</script>

<template>
  <h2>First message {{msg}}</h2>
</template>

<style scoped>
  h2{
    background: green;
  }
</style>