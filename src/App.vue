<template>
  <div class="back">
    <navbar-vue></navbar-vue>
  </div>
  <Footer></Footer>
</template>
<script>
import navbarVue from "./components/navbar.vue";
import Footer from "./components/foot.vue"

export default{
  components:{
    navbarVue,
    Footer,
}
}
</script>

<style scoped>
*{
  margin: 0; 
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  color: #2c3e50;
}
.back{
  background-image: url("https://i.postimg.cc/jjm4fL79/golden-clouds-duncan1890.jpg");
  
    background-position: center;
    background-size: cover;
    height: 90vh;
    background-attachment: fixed;
    position: relative;
  
}



</style>
