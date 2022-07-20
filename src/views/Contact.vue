<template>
  <div id="contact">

      <div class="container container-fluid  ">
          <div class="row justify-content-center">
              <div class="col-12 text-center">
                  <div class="container-title text-center mb-4">
                      <div class="titles mt-3">
                          <h2 class="title text-capitalize mb-4 text-light">Contact</h2>
                          <p class="pera-title para-desc-600 text-light mb-0 mx-auto"></p>
                          <span></span>
                      </div>
                  </div>
              </div>
          </div>

          <div class="row">
              <div class="col-md-4 mt-1 pt-1">
                  <div class="contact-detail text-center">
                      <div class="icon text-light">
                          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-phone fea icon-md"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg>
                      </div>
                      <div class="content mt-4">
                          <h5 class="title text-light">Phone</h5>
                          <p class="text-light">For any business enquiries please feel free to Contact me on this number.</p>
                          <a href="tel:+152534-468-854" class="text-light">+27 72 068 1768</a>
                      </div>  
                  </div>
              </div>
              
              <div class="col-md-4 mt-1 pt-1">
                  <div class="contact-detail text-center">
                      <div class="icon text-light">
                          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail fea icon-md"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
                      </div>
                      <div class="content mt-4">
                          <h5 class="title text-light">Email</h5>
                          <p class="text-light">Drop me an Email and let's talk business!</p><br>
                          <a href="mailto:contact@example.com" class="text-light">ikhlaas21.rawoot@gmail.com</a>
                      </div>  
                  </div>
              </div>
              
              <div class="col-md-4 mt-1 pt-1">
                  <div class="contact-detail text-center">
                      <div class="icon text-light">
                          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-map-pin fea icon-md"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
                      </div>
                      <div class="content mt-4">
                          <h5 class="title text-light">Location</h5>
                          <p class="text-light">Cape Town, South Africa</p><br>
                          <a href="https://goo.gl/maps/5f4wN5GkMfVBzqgs7" target="_blank" class="map-popup-view text-light">View on Google maps</a>
                      </div>  
                  </div>
              </div>
          </div>
      </div>
     <section class="section pt-1">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-12">
                    <div class="custom-form mb-sm-30">
                        <form method="post" action="https://formspree.io/f/xdobyzlo" name="myForm" onsubmit="return validateForm()">
                            <p id="error-msg"></p>
                            <div id="simple-msg"></div>
                            <div class="row">
                                <div class="col-lg-6">
                                    <div class="row">
                                        <div class="col-lg-12 col-md-6 mt-2">
                                            <div class="form-group">
                                                <input name="name" id="name" type="text" class="form-control border rounded" placeholder="First Name :">
                                            </div>
                                        </div>
                                        <div class="col-lg-12 col-md-6 pt-2">
                                            <div class="form-group">
                                                <input name="email" id="email" type="email" class="form-control border rounded" placeholder="Your email :">
                                            </div> 
                                        </div>
                                       
                                    </div>
                                </div>

                                <div class="col-lg-6 mt-2">
                                    <div class="form-group">
                                        <textarea name="comments" id="comments" rows="3" class="form-control border rounded" placeholder="Your Message :"></textarea>
                                    </div>
                                </div>
                            </div>
                            <div class="row">
                                <div class="col-sm-12 text-center pt-3 pb-2">
                                    <input type="submit" id="submit" name="send" class="submitBnt btn btn btn-light rounded" value="Send Message"> 
                                </div>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
*{
    z-index: -3;
}
.container{
    width: 800px
}
#contact{
    background-color: maroon;
    border: solid 5px maroon;
    border-radius: 20px;
  

}
form input[type=text] {
background-color:cornsilk;
}

form input[type=email] {
background-color:cornsilk;
}

form #comments{
background-color: cornsilk;
}
.text-light {
    color: rgb(253, 216, 141) !important;
}
input{
    color: black;
    background-color: blanchedalmond
}

</style>