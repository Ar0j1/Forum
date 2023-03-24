<template>
  <ul>
    <FirstScreenMenuItem
        v-for="MenuItem of MenuItems" :key='MenuItem.id'
        v-bind:MenuItem = 'MenuItem'
    />
  </ul>

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

  ul{
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }


</style>