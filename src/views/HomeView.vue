<template>
  <div class="home">
    <div id="land" class="container container-fluid d-flex justify-content-center align-items-center flex-column  ">
      <img id="suit" src="https://i.postimg.cc/vHx8nvcz/cropme.jpg" alt="me" defer>
      <h1>Ikhlaas Rawoot</h1>
      <h3>
        <a href="" style="color: rgb(0,0,0) ;" class="typewrite" data-period="2000"
          data-type='[ "An Aspiring Web Developer 🤩", "I Love 3D Printing 💕", "" ]' />
        <span class="wrap"></span>
        </h3>
        <br>
        <br>
        
      
    </div>
      
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
*{
  z-index: -3;
  }

h1{
  text-align: center;
  color: black;
  font-size: 48px;
  padding-top: 10px;
}
#suit {
    width: 220px;
    height: 220px;
    border: 7px solid #800000;
    border-radius: 50%;
    z-index: 2;
    object-fit: cover;
    

}
a{
  width: 100%;
    /* color: black; */
  display: flex;
  justify-content: center;
  align-content: center;
  
}
a.typewrite{
  width: 350px;
  height: 30px;

}

#land{

  height: 35vh;
  display: flex;
  
  
}
</style>



