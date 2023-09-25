<script setup>
  const ok = false
  const notOkay = true
  const msg = "if okay is true this message will be shown"
</script>

<template>
   <h1 v-if="ok">{{msg + ok}}</h1>
   <h1 v-if="notOkay">{{msg + ok}}</h1>
</template>