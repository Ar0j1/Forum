<template>
  <li>
    {{MenuItem.title}}
  </li>
</template>

<script>
export default {
  props: {
    MenuItem:{
      type: Object,
      required:true
    }
  },
  name: "FirstScreenMenuItem"
}
</script>
<style scoped>

</style>