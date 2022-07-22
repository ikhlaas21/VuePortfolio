<template>
    <div class="resume">
        <div class="container">
            <div class="wrap animate pop">
	<div class="overlay">
		<div class="overlay-content animate slide-left delay-2">
			<h2 class="animate slide-left pop delay-4">Resume</h2>
			<p class="animate slide-left pop delay-5" style=" margin-bottom: 2.5rem; margin-left: 0.4rem;">Hover <em>Here</em></p>
		</div>
		<div class="image-content animate slide delay-5"></div>
		<!-- <div class="dots animate">
			<div class="dot animate slide-up delay-6"></div>
			<div class="dot animate slide-up delay-7"></div>
			<div class="dot animate slide-up delay-8"></div>
		</div> -->
	</div>
	<div class="text">
        
        <h3>Work Experience</h3>
		 <h5>{{work[0].title}}</h5>
             {{work[0].text}}
        <hr>
        <h3>Education</h3>
        <h5>{{education[0].title}}</h5>
        {{education[0].text}}
        <hr>
    
        <h5>{{education[1].title}}</h5>
        {{education[1].text}}
            
	</div>
</div>
            <!-- <div class="row mx-auto">


                <div id="one" class="col-6 ms-auto">
                    <div id="card1" class="card ">
                        <div class="card-body">
                            <h3 class="card-header">Education</h3>
                            <div class="card-thorax">
                                <p class="card-text ">
                                <h5>Life Choices Academy</h5>
                                Currently studying Web Development - 2022
                                <h5>Livingstone High School</h5>
                                Attended Livingstone for 5 years where I acquired my Matric Certificate - 2016 to 2020
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
                <div id="two" class="col-6 me-auto">
                    <div id="card2" class="card ">
                        <div class="card-body">
                        <h3 class="card-header">Work Experience</h3>
                                <div class="card-thorax">
                                <p class="card-text">
                                    <br>
                                <h5>PRINGLE OF SCOTLAND</h5>
                                Worked in retail as a Sales Assistant(Casual)
                                - December 2021 to January 2022
                                </p>
                            </div>
                            <br>
                        </div>
                    </div>
                </div>
                 <div id="three" class="col-4">
            </div>


            </div> -->
        </div>
    </div>

</template>

<script>
export default {
     computed:{
        work(){
            return this.$store.state.work
        },
        education(){
            return this.$store.state.education
        }        
       
     }
}
</script>

<style scoped>
/* *{
    z-index: -2;
} */
h2 {
	font-size: 4.8vmin;
	text-align: center;
	color:rgb(253, 216, 141);
}
p {
	font-size: max(10pt, 2.5vmin);
	line-height: 1.4;
    text-shadow: 5px 5px 20px  black;
	margin-bottom: 1.5rem;
    color: rgb(253, 216, 141);
}

.wrap {
	display: flex;
	flex-wrap: nowrap;
	justify-content: space-between;
	width: 85vmin;
	height: 26em;
	border: 8px solid maroon;
    
	/* border-image: linear-gradient(-50deg,maroon, rgb(253, 216, 141), maroon,rgb(253, 216, 141), maroon,rgb(253, 216, 141),maroon) 1; */
	margin: 2rem auto;
    border-radius: 10px;
	transition: .3s ease-in-out;
	position: relative;
	overflow: hidden;
    
}
.overlay {
	position: relative;
	display: flex;
	width: 100%;
	height: 100%;
	padding: 1rem .75rem;
	background:maroon;
	transition: .4s ease-in-out;
	z-index: 1;
}
.overlay-content {
	display: flex;
	flex-direction: column;
	justify-content: space-between;
	width: 15vmin;
	height: 100%;
	padding: .5rem 0 0 .5rem;
	border: 3px solid;
	border-image: 
    	linear-gradient(
      	to bottom, 
      	rgb(253, 216, 141) 5%,
      	maroon 35% 65%,
      	rgb(253, 216, 141) 95%
    	) 0 0 0 100%;
	transition: .3s ease-in-out .2s;
	z-index: -2;
}
.image-content {
	position: absolute;
	top: 0;
	right: 0;
	width: 56vmin;
	height: 100%;
	background-image: url("https://i.postimg.cc/3J760f52/F08CWK.webp");
	background-size: cover;
	transition: .3s ease-in-out;
    z-index: -5;
	/* border: 1px solid green; */
}

.dots {
	position: absolute;
	bottom: 1rem;
	right: 2rem;
	display: flex;
	flex-direction: row;
	justify-content: space-around;
	align-items: center;
	width: 55px;
	height: 4vmin;
	transition: .3s ease-in-out .3s;
}
.dot {
	width: 14px;
	height: 14px;
	background:rgb(253, 216, 141);
	border: 1px solid maroon;
	border-radius: 10px;
	transition: .3s ease-in-out .3s;
}

.text {
	position: absolute;
	top: 0;
	right: 0;
	width: 60vmin;
	height: 100%;
	padding: 3vmin 4vmin;
	background: rgb(253, 216, 141);
	box-shadow: inset 1px 1px 15px 0 rgba(0 0 0 / .4);
	
}

.wrap:hover .overlay
 {
	transform: translateX(-60vmin);
}
.wrap:hover .image-content {
	width: 30vmin;
}
.wrap:hover .overlay-content {
	border: none;
	transition-delay: .2s;
	transform: translateX(60vmin);
}
.wrap:hover .dots {
	transform: translateX(1rem);
}
.wrap:hover .delay-5 {
	/* background:rgb(253, 216, 141); */
    color: black;
}

.wrap:hover> .overlay > .overlay-content > p{
    color: black
}


/* Animations and timing delays */
.animate {
  animation-duration: 0.7s;
  animation-timing-function: cubic-bezier(.26, .53, .74, 1.48);
  animation-fill-mode: backwards;
}
/* Pop In */
.pop { animation-name: pop; }
@keyframes pop {
  0% {
    opacity: 0;
    transform: scale(0.5, 0.5);
  }
  100% {
    opacity: 1;
    transform: scale(1, 1);
  }
}

/* Slide In */
.slide { animation-name: slide; }
@keyframes slide {
  0% {
    opacity: 0;
    transform: translate(4em, 0);
  }
  100% {
    opacity: 1;
    transform: translate(0, 0);
  }
}

/* Slide Left */
.slide-left { animation-name: slide-left; }
@keyframes slide-left {
  0% {
    opacity: 0;
    transform: translate(-40px, 0);
  }
  100% {
    opacity: 1;
    transform: translate(0, 0);
  }
}

.slide-up {animation-name: slide-up;}
@keyframes slide-up {
	0% {
		opacity: 0;
		transform: translateY(3em);
	}
	100% {
		opacity: 1;
		transform: translateY(0);
	}
}

.delay-1 {
  animation-delay: 0.3s;
}
.delay-2 {
  animation-delay: 0.6s;
}
.delay-3 {
  animation-delay: 0.9s;
}
.delay-4 {
  animation-delay: 1.2s;
}
.delay-5 {
  animation-delay: 1.5s;
}
.delay-6 {
  animation-delay: 1.8s;
}
.delay-7 {
  animation-delay: 2.1s;
}
.delay-8 {
  animation-delay: 2.4s;
}
/*
.row {
    height: 400px;
    width: 1000px;
}

.card-thorax {
    display: none;
    transition: 5s ease-in-out;
}

.card {
    border: solid 2px maroon;

}

.col-6 {
    width: 250px;
    height: 405px;
    z-index: 0;
    transition: 0.5s;


}
#card2{
    height: 400px;
}
#card1{
    height: 400px;
}

.col-6:hover {
    width: 750px;
    z-index: 1;
}
.col-6:hover .card-thorax{
    display: block;
    transition: 5s ease-in-out;
}
*/

/* .resume{
    height: 150vh;
} */
/* #one{
    margin-left: 100px;
}
#two{
    width: 50px;
}
#three{
    margin-right: 100px;
} */
</style>