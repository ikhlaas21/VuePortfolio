<template>
    <div class="container container-fluid">
        <input type="checkbox" id="checkbox" >
        <div class="toggle" @click="handleEvent">
        <span class="top_line common"></span>
        <span class="middle_line common"></span>
        <span class="bottom_line common"></span>
        </div>


        <div class="slide">
            <nav>
                <router-link to="/">Home</router-link>
                <hr>
                <router-link to="/about">About</router-link>
                <hr>
                <router-link to="/resume">Resume</router-link>
                <hr>
                <router-link to="/skills">Skills</router-link>
                <hr>
                <router-link to="/testimonials">Testimonials</router-link>
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
        <!-- <input type="color" v-model="color">
    {{color}} -->
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

export default {
    components: {
        Footer,
    },
    // methods: {
    //     changeColor() {
    //         document.querySelector(":root")
    //     }
    // },
    data() {
        return {
            isChecked: false
        }
    },
    methods: {
        handleEvent() {
            this.isChecked = !this.isChecked;
            console.log(this.isChecked)
            if(this.isChecked == true){
                document.querySelector("#checkbox").checked = true;
             document.querySelector('.slide').style.transform= "translateX(0px)";
             document.querySelector('.slide').style.transition= "all 0.8s ease";
            }
            if (this.isChecked == false){
                document.querySelector("#checkbox").checked = false;
             document.querySelector('.slide').style.transform= "translateX(-180px)"
            }
        }
    }
}
</script>

<style scoped>
* {
    margin: 0;
    padding: 0;
    font-family:'Crimson Text', serif;   
}

.slide{
    position: relative;
}
.slide::after{
    content: '';
    position: absolute;
    z-index: 1;
}

.slide>nav{
    z-index: 100;
}

nav {
    position: absolute;
    padding: 15px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-radius: 10px;
    background-color: maroon;
    border: solid 5px rgb(253, 216, 141);
    /* border-bottom: none; */
    height: 100vh;
    width: 180px;
    font-size: larger;
   
     z-index: 1;
}

nav a {
    font-weight: bold;
    color: rgb(253, 216, 141);
    padding-top: 20px;
    font-size: 23px;
    /* padding-bottom: 20px; */
    text-decoration: none;


}

/* .fff{
    display: flex;
    color: ;
    justify-content: baseline;
} */
a:hover {

    color: maroon;
    background-color: rgb(253, 216, 141);
    border-radius: 5px;
    height: 55px;
    padding: 0;
    padding-top: 10px;
    padding-left: 9px;
    transition: 0.5s;
}

hr {
    color: rgb(253, 216, 141);

}

main {
    height: 100%;
    display: grid;
    place-content: center;
}

.route-enter-from {
    opacity: 0;
    transform: translateX(-200px);
}

.route-enter-active {
    transition: all 0.5s ease-out;
}

.route-leave-to {
    opacity: 0;
    transform: translateX(1500px);
}

.route-leave-active {
    transition: all 0.5s ease-in;
}

:root {
    --background-color: #fffaff;
    --text-color: #333;

}
input{
display: none;
visibility: hidden ;
-webkit-appearance: none;
}
.toggle{
    position: absolute;
    height:30px;
    width: 30px;
    top: 15px;
    left: 11px;
    z-index: 25;
    cursor: pointer;
    border-radius: 5px;
    background-color: rgb(253, 216, 141);
    box-shadow: 0 0 10px rgba(0,0,0,0.3);
}
.toggle .common{
    position: absolute;
    height: 2px;
    width: 25px;
    background-color: maroon;
    border-radius: 50px;
    transition: 0.3s ease;
    left:0;
}
.toggle .top_line{
    top: 30%;
    left: 50%;
    transform: translate(-50%,-50%);
}
.toggle .middle_line{
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
}
.toggle .bottom_line{
    top: 70%;
    left: 50%;
    transform: translate(-50%,-50%);
}
.slide{
   transform: translateX(-180px); 
   z-index: 24;
}
input:checked ~ .toggle .top_line{
    left: 2px;
    top: 14px;
    width: 25px;
    transform: rotate(45deg);
}
input:checked ~ .toggle .bottom_line{
    left: 2px;
    top: 14px;
    width: 25px;
    transform: rotate(-45deg);
}
input:checked ~ .toggle .middle_line{
   opacity: 0;
    transform: translateX(20px);
}
input:checked ~ .slide{
    transform:translateX(0)
}
</style>