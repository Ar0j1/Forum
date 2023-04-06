<template>
    <div id="el">
        <img :src="ItemOfForm.image"/>
        <p class="date">{{ ItemOfForm.date }}</p>
        <p id="red">{{ ItemOfForm.title }}</p>
        <p>{{ ItemOfForm.description }}</p>
      </div>

</template>
  
<script>
  export default {
  name: "ItemOfForm",
  props:["ItemOfForm"],
  data(){
    return{
        
    }
  }

}
</script>
  
<style>
</style>