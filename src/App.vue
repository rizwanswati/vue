<script setup>

import Text from "@/components/Text.vue";
</script>

<template>
  <Text msg="Hello World" rawhtml="<span style=color:red>" dynamic-i-d="alpha101" data-number="105" disability="disabled"></Text>
  <Text msg="Hello World" rawhtml="<span style=color:red>" dynamic-i-d="alpha101" data-number="105" disability=""></Text>
  <Text msg="Hello World" rawhtml="<span style=color:red>" dynamic-i-d="alpha101" data-number="105"></Text>

  <Text id="505" class="container" itemID="105" dataID="56"></Text>
</template>