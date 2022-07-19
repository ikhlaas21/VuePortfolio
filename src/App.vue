<template>

  <div class="back">
    <navbar-vue></navbar-vue>
  <div class="move">
        <div class="icons">
          <a href="https://github.com/ikhlaas21"><i class="bi bi-github"></i> </a>
          <a href="https://www.instagram.com/ikhlaas21/"><i class="bi bi-instagram"></i></a>
          <a href="https://www.linkedin.com/in/ikhlaas-rawoot-531a71201/"><i class="bi bi-linkedin"></i></a>
          <a href="https://seranking.com/blog/wp-content/uploads/2021/01/404_01-min.jpg"><i class="bi bi-twitter"></i></a>
        </div>

      </div>
  </div>
</template>
<script>
import navbarVue from "./components/navbar.vue";


export default{
  components:{
    navbarVue,
    
}
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@1,600&display=swap');
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
    height: 100vh;
    background-attachment: fixed;
    position: relative;
     overflow-x: hidden;
  overflow-y: hidden;
  
}
.icons{
  height: 220px;
  width: 70px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  text-align: center;
  /* flex-direction: column; */
  color: rgb(253, 216, 141) ;
  background-color: #800000 ;
  z-index: 2;
  border: solid rgb(253, 216, 141)5px;
  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
  border-right: none;
  font-size: 30px;
  padding-top: 2px;


  
  
}
.bi{
   color: rgb(253, 216, 141) ;
  
}
.bi:hover{
  color:black;
}
.move{
  display: flex;
  justify-content: flex-end;
  position: fixed;
  right: 0;
  bottom: 10%
}



</style>
