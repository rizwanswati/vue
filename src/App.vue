<script setup>
  import Attribinding from "@/components/Attribinding.vue";

  const ok = false
  const notOkay = true
  const msg = "if okay is true this message will be shown"
  const text = "this is a text message"
  function doSomething(){
    console.log('clicking')
  }
</script>

<template>
   <h1 v-if="ok">{{msg + ok}}</h1>
   <h1 v-if="notOkay">{{msg + ok}}</h1>

  <button v-on:click="doSomething">Click it</button>
  <div>{{text}}</div>

  <Attribinding attrname="href" url="www.google.com" eventname="focus"></Attribinding>
</template>