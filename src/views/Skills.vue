<template>
  <div class="container container-fluid ">
      <h1>Work Expertise</h1>
      <h6>I am a Young Programmer at the beginning of my journey</h6>
      <br>
      
    <div class="row" >
        <div class="col-sm-6">
          <img class="img-fluid" src="https://i.postimg.cc/Tw6mKcpH/IMG-1145.jpg" alt="me">
        </div>
        <div class="col-sm-6">
            <h3>Technical Skills</h3>
        <div>
              <p class="d-flex justify-content-between pt-1">
                HTML <span>80%</span>
              </p>
              <div class="progress">
                <div class="progress-bar progress-bar-animated progress-bar-striped" role="progressbar"
                  style="width: 80%" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
            <div>
              <p class="d-flex justify-content-between">
                CSS <span>85%</span>
              </p>
              <div class="progress">
                <div class="progress-bar  progress-bar-animated progress-bar-striped" role="progressbar"
                  style="width: 85%" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
            <div>
              <p class="d-flex justify-content-between">
                Bootstrap <span>70%</span>
              </p>
              <div class="progress">
                <div class="progress-bar  progress-bar-animated progress-bar-striped" role="progressbar"
                  style="width: 70%" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
            <div>
              <p class="d-flex justify-content-between">
                JavaScript <span>45%</span>
              </p>
              <div class="progress">
                <div class="progress-bar  progress-bar-animated progress-bar-striped" role="progressbar"
                  style="width: 45%" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
             <div>
              <p class="d-flex justify-content-between">
                MySQl <span>68%</span>
              </p>
              <div class="progress">
                <div class="progress-bar  progress-bar-animated progress-bar-striped" role="progressbar"
                  style="width: 68%" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
              </div>
            </div>
            <br>
            <h3>Soft Skills</h3>
             <div class="soft">
                    <h5>Leadership Skills</h5>
                 <h5>Interpersonal Skills</h5>
             </div>
             <div class="soft">
                 <h5>Problem-Solving</h5>   
                 <h5>TeamWorking Skills</h5>
             </div>
              
             <!-- <router-link to="/skills2"><button>View More</button></router-link> -->
                          <router-link to="/skills2"><button>View More</button></router-link>

        </div>
    </div>
  </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.container{
    width: 700px;
    margin-top: -50px;
}
img{
    width: 370px;
    height: 505px;
}
h1{
    text-align: center;
    font-size: 60px;
}
h6{
    text-align: center;
}
.progress-bar {
    background-color: maroon;
}
.soft{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
h5{
    height: 32px;
    transition: 0.4s;
}
h5:hover{
    background-color: rgb(253, 216, 141);
    border: solid 5px rgb(253, 216, 141);
    border-radius: 5px;
    height: 32px;
}
button{
    background-color:rgb(253, 216, 141);
    width: 100px;
    height: 35px;
    color: #222;
    border: solid 3px maroon;
    border-radius: 3px;
    transition: 0.5s;

}
button:hover{
     color: maroon;
    border: solid 3px rgb(253, 216, 141);
    border-radius: 3px rgb(253, 216, 141);
     background-color: rgb(253, 216, 141);
     transform: translateX(10px);
}
/* vue transition */

</style>