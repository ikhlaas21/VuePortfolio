<template>
<div class="container">
   
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
      <router-link to="/about">Contact</router-link>
      <hr>
      
    </nav>

</div>
  <router-view/>
</template>

<style scoped>
*{
  margin: 0; 
  padding: 0;
}

nav {
  padding: 30px;
  display:flex;
  flex-direction: column;
  justify-content: center;
  border:solid 2px;
  background-color: maroon;
  border:solid 5px rgb(253, 216, 141);
  border-bottom: none;
  height:90vh ;
  width:fit-content;
  font-size: larger;
  position: absolute;
  
}

nav a {
  font-weight: bold;
  color: rgb(253, 216, 141);
  padding-top:20px;
  /* padding-bottom: 20px; */
  text-decoration: none;
  
  
}

/* nav a.router-link-exact-active {
  color: #42b983;
} */

</style>