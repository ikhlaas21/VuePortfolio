<template>
<div class="about">
  <div class="uno">
    <h1>About Ikhlaas..</h1>
  </div>
    
    
  <div class="ab container">

    <div id="aboutcard" class="container container-fluid">
      
      <div class="card-group">
        <div class="card ">
          <!-- <img src="..." class="card-img-top" alt="..."> -->
          <div class="card-body">
            <h5 class="card-title">Personal Details:</h5>
            
            <hr>
          <br>
            <p class="card-text">
              <ul id="aboutlist">
                <li><b>Full name:</b> Ikhlaas Ahmed Rawoot</li>
                <li><b>Date of birth:</b> 21/08/2002</li>
                <li><b>Gender:</b> Male</li>
                <li><b>Location:</b> Grassy Park</li>
                <li><b>Cell Phone number:</b> 072 086 1768</li>
                <li><b>Email Address:</b> ikhlaas21.rawoot@gmail.com</li>
                <li><b>Willing to Relocate:</b> No</li>
              </ul>
            </p>

          </div>
        </div>
        <div class="card">
          <!-- <img src="..." class="card-img-top" alt="..."> -->
          <div class="card-body">
            <h5  class="card-title" style="color: maroon;"> Bio<a href="" style="color: maroon ;"/>
              <span class="wrap"></span>
              </h5>
              
            <p class="card-text pt-1">I enjoy the company of others and have excellent teamwork skills. Although I am a team
              player, I also have the ability to take the lead when necessary. I see failure as a lesson learnt and
              never shy from trying again. I would like to think that I am resilient and hardworking.
              <br> I am extremely
              passionate about modern technology and have recently started a 3D printing business with my brother. In 3D
              printing, there is a lot of trial and error. In order to be successful in this field, one needs to be
              patient and show perseverance.</p>

          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<style scoped>
*{
  margin: 0; 
  padding: 0;
  z-index: -3;
}
h1{
  text-align: center;
}
#aboutlist {
    list-style: none;
    font-size: 19px;
    
}
#aboutcard{
 
  height: 35vh;
  display: flex;
  width: 900px;
  display: flex;
 
}
.ab{
  display: flex;
  justify-content: center;
  margin-bottom: 150px;
  
}
.card{
  background-color:rgb(253, 216, 141);
  border: solid 3px maroon;
  min-height: 330px;
}
.card-text{
   padding:10px;
   font-size: 19px;
   


}


.card-title{
  font-weight: bold;
}
.card-body{
  padding: 10px;
}
h1{
   text-align: center;
   font-size: 70px;
}
.uno{
  margin-bottom: 50px;
}

@media (max-width: 321px) {
    .container{
        width: 280px;
        /* height: fit-content; */
        margin-left: 10px;
       
    }
    .card{
      height: fit-content;
    }
    h1{
      margin-top: 30px;
    }
}
@media (max-width: 426px) {
    .container{
        width: 280px;
        /* height: fit-content; */
        margin-left: 10px;
       
    }
    .card{
      height: fit-content;
    }
    h1{
      margin-top: 30px;
    }
}

</style>
