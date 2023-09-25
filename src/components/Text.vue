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
    },
    dataNumber:{
      required: true,
      type: String
    },
    disability:{
      type: Boolean,
      required: true
    },
  })
  const properties = {
    id: "test-101",
    class: "container",
    dataID: "10",
    itemID: "05"
  }
</script>

<template>
<!--  Interploate plain text -->
  <h2>First message {{msg}}</h2>

<!--  give out raw html-->
  <h2>this is html <span v-html="rawhtml"></span></h2>

<!--  attribute binding-->
  <div v-bind:id="dynamicID">this contains a dynamic id {{dynamicID}}</div>

<!--  Dynamic binding shorthand-->
  <div :itemid="dataNumber">dynamic binding shorthand :attr {{dataNumber}}</div>

<!--  True or False attributes-->
  <button :disabled="disability">Disabled</button>
  <button :disabled="disability">Enabled</button>

<!--  Multiple properties binding-->
  <div v-bind="properties">{{properties}}</div>


</template>

<style scoped>
  h2{
    background: green;
  }
</style>