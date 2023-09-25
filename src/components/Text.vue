<!--
  - {{}} will translate everything into simple plain text.
  - if there is need to output actual html then v-html directive should be use, see below example
-->
<script setup>
  defineProps({
    msg:{
      required:true,
      type:String
    },
    rawhtml:{
      required: true
    },
    dynamicID:{
      required: true,
      type:String
    }
  })
</script>

<template>
<!--  Interploate plain text -->
  <h2>First message {{msg}}</h2>

<!--  give out raw html-->
  <h2>this is html <span v-html="rawhtml"></span></h2>


<!--  attribute binding-->
  <div v-bind:id="dynamicID">this contains a dynamic id</div>
</template>

<style scoped>
  h2{
    background: green;
  }
</style>