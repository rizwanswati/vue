<script setup>
  defineProps(
      {
        attrname:{
          type:String
        },
        url:{
          type:String
        },
        eventname:{
          type:String
        }
      }
  )
  function doSomething(){
    console.log('focusing')
  }
</script>

<template>
<!--  both are same-->
  <a v-bind:[attrname] = "url" target="_blank">Google</a>
  <a :[attrname] = "url" target="_blank">Google</a>
  <a v-on:[eventname] = "doSomething" v-bind:[attrname] = "url">Facebook</a>
</template>

<style scoped>

</style>