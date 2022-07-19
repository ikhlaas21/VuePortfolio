<template>
  <div class="about">
   
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
                <li>Full name: Ikhlaas Ahmed Rawoot</li>
                <li>Date of birth: 21/08/2002</li>
                <li> Gender: Male</li>
                <li>Location: Grassy Park</li>
                <li>Cell Phone number: 072 086 1768</li>
                <li>Email Address: ikhlaas21.rawoot@gmail.com</li>
                <li>Willing to Relocate: No</li>
              </ul>
            </p>

          </div>
        </div>
        <div class="card">
          <!-- <img src="..." class="card-img-top" alt="..."> -->
          <div class="card-body">
            <h5 class="card-title"> <a href="" style="color: maroon ;" class="typewrite" data-period="2000"
                data-type='[ "Bio" ]' />
              <span class="wrap"></span>
              </h5>
              <br>
            <p class="card-text">I enjoy the company of others and have excellent teamwork skills. Although I am a team
              player, I also have the ability to take the lead when necessary. I see failure as a lesson learnt and
              never shy from trying again. I would like to think that I am resilient and hardworking. I am extremely
              passionate about modern technology and have recently started a 3D printing business with my brother. In 3D
              printing, there is a lot of trial and error. In order to be successful in this field, one needs to be
              patient and show perseverance.</p>

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
}
h1{
  text-align: center;
}
#aboutlist {
    list-style: none;
    
}
#aboutcard{
  
  height: 35vh;
  display: flex;
  width: 800px;
  display: flex;
  

  
  
  
}
.about{
  display: flex;
  justify-content: center;
  
  
}
.card{
  background-color:rgb(253, 216, 141);
  border: solid 3px maroon;
  height: 300px;
}

.card-body{
  padding: 10px;
}

</style>
