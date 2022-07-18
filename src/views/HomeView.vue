<template>
  <div class="home">
    <h1>THIS WILL BE THE HOME</h1>
  </div>
  
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>

h1{
  text-align: center;
}
</style>
