<script setup>
  defineProps(
      {
        attrName:{
          type:String
        },
        url:{
          type:String
        }
      }
  )
</script>

<template>
<!--  both are same-->
  <a v-bind:[attrName] = "url" target="_blank">Google</a>
  <a :[attrName] = "url" target="_blank">Google</a>
</template>

<style scoped>

</style>