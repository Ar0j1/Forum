<template>
  <div id="upperbox">
    <FirstScreenMenuItem
        v-for="MenuItem of MenuItems" :key='MenuItem.id'
        v-bind:MenuItem = 'MenuItem'
    />
  </div>

</template>

<script>
import FirstScreenMenuItem from './FirstScreenMenuItem.vue';

export default {
  props:['MenuItems'],

  name: "FirstScreenMenu",
  components: {
    FirstScreenMenuItem
  }
}
</script>

<style scoped>

  #upperbox{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
  }


</style>