<template>
<div class="container container-fluid">
   
    <nav>
      <router-link to="/">Home</router-link> 
      <hr>
      <router-link to="/about">About</router-link>
      <hr>
      <router-link to="/">Resume</router-link> 
      <hr>
      <router-link to="/about">Skills</router-link>
      <hr>
       <router-link to="/about">Testimonials</router-link>
       <hr>
      <router-link to="/">Projects</router-link> 
      <hr>
      <router-link to="/contact">Contact</router-link>
      <hr>
      <div class="fff">
          <Footer></Footer>

      </div>
      
    </nav>

</div>
<main>
    <router-view v-slot="{ Component }">
      <transition name="route" mode="out-in">
          <component :is="Component"></component>
      </transition>
    </router-view>

</main>
</template>
<script>
import Footer from "./foot.vue"

export default{
  components:{
     Footer,
}
}
</script>

<style scoped>
*{
  margin: 0; 
  padding: 0;
  font-family: 'Crimson Text', serif;
}

nav {
  padding: 30px;
  display:flex;
  flex-direction: column;
  justify-content: center;
  border-radius:10px;
  background-color: maroon;
  border:solid 5px rgb(253, 216, 141);
  /* border-bottom: none; */
  height:100vh ;
  width:fit-content;
  font-size: larger;
  position: absolute;
  z-index: 3;
}

nav a {
  font-weight: bold;
  color: rgb(253, 216, 141);
  padding-top:20px;
  font-size: 23px;
  /* padding-bottom: 20px; */
  text-decoration: none;
  
  
}

/* .fff{
    display: flex;
    color: ;
    justify-content: baseline;
} */
a:hover{
  
    color: maroon;
    background-color: rgb(253, 216, 141) ;
    border-radius: 5px;
    height: 55px;
    padding: 0;
    padding-top: 10px;
    padding-left: 15px;
}

hr{
    color: rgb(253, 216, 141);

}
main{
        height: 100%;
    display: grid;
    place-content: center;
}

.route-enter-from{
    opacity: 0;
    transform: translateX(-200px);
}

.route-enter-active{
    transition: all 0.5s ease-out;
}
.route-leave-to{
    opacity: 0;
    transform: translateX(1500px);
}
.route-leave-active{
    transition: all 0.5s ease-in;
}

</style>