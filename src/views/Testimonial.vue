<template>
<div class="testimonials">

    <section class="pn_reviews my-5">
    <div class="container">
        <div class="row">
            <div class="col-md-12">
                <h1 class="text-center pb-5">I made some changes</h1>
            </div>

            <div class="col-md-12 col-lg-4">
                <div class="pn_testimonial_box mt-4">
                    <p class="text-justify">What does Lorem Ipsum mean? Derived from Latin dolorem ipsum (“pain itself”), Lorem Ipsum is filler text used by publishers and graphic designers used to demonstrate graphic elements.
</p>

                    <div class="row pt-3">
                        <div class="col-md-6 pn_review_profile"><img src="https://desklib.com/static/src/assets/images/v2/profile_1.svg" class="border-radius-12 float-right" alt="client image" /> <span> Charles Boyle </span> </div>
                        <div class="col-md-6 pn_review_rating d-flex justify-content-end"> 5 &nbsp; <img class="image-radius aligncenter" src="https://desklib.com/static/src/assets/images/v2/star_rating.svg" alt="client stars image" /> </div>
                    </div>
                </div>
            </div>
            <div class="col-md-12 col-lg-4">
                <div class="pn_testimonial_box mt-4">
                    <p class="text-justify">What does Lorem Ipsum mean? Derived from Latin dolorem ipsum (“pain itself”), Lorem Ipsum is filler text used by publishers and graphic designers used to demonstrate graphic elements.
</p>
                    <div class="row pt-3">
                        <div class="col-md-6 pn_review_profile"><img src="https://desklib.com/static/src/assets/images/v2/profile_2.svg" class="border-radius-12 float-right" alt="client image" /> <span> Gina Lannety </span> </div>
                        <div class="col-md-6 pn_review_rating d-flex justify-content-end"> 5 &nbsp; <img class="image-radius aligncenter" src="https://desklib.com/static/src/assets/images/v2/star_rating.svg" alt="client stars image" /> </div>
                    </div>
                </div>
            </div>
            <div class="col-md-12 col-lg-4">
                <div class="pn_testimonial_box mt-4">
                    <p class="text-justify">What does Lorem Ipsum mean? Derived from Latin dolorem ipsum (“pain itself”), Lorem Ipsum is filler text used by publishers and graphic designers used to demonstrate graphic elements.
 </p>
                    <div class="row pt-3">
                        <div class="col-md-6 pn_review_profile"><img src="https://desklib.com/static/src/assets/images/v2/profile_3.svg" class="border-radius-12 float-right" alt="client image" /> <span> Dug Judey </span> </div>
                        <div class="col-md-6 pn_review_rating d-flex justify-content-end"> 5 &nbsp; <img class="image-radius aligncenter" src="https://desklib.com/static/src/assets/images/v2/star_rating.svg" alt="stars image" /> </div>
                    </div>
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
.container{
    width: 900px;
    margin-top: -50px;
}
.pn_testimonial_box {
  font-weight: 300;
  padding: 2rem;
  margin: 2rem;
  border: 1px solid #405fbd;
  position: relative;
  transition: 1s;
  transform: scale(0.9);
  background-color: #fff;
  -webkit-border-radius: 4rem;
  -moz-border-radius: 4rem;
  -ms-border-radius: 4rem;
  border-radius: 4rem;
}
.pn_testimonial_box:hover {
  box-shadow: 2px 4px 8px #d6d8da;
  border: 1px solid #fff;
  transform: scale(1);
  position: relative;
  z-index: 1;
}
.pn_review_rating img {
  width: 20%;
}
.pn_review_profile img {
  position: absolute;
  margin: -1rem -5rem 0;
}
.pn_review_profile span {
  position: absolute;
}


@media (max-width: 575px) {
    /*---------- testimonial css start ----------*/
    .pn_reviews {
        padding: 3rem 0;
    }
    .pn_reviews h1 {
        font-size: 2rem;
        padding-bottom: 1rem !important;
    }
    .pn_testimonial_box {
        padding: 2rem;
        margin: 1rem;
        border: 1px solid #405fbd;
        position: relative;
        -webkit-border-radius: 4rem;
        -moz-border-radius: 4rem;
        -ms-border-radius: 4rem;
        border-radius: 4rem;
    }
    .pn_review_profile img {
        position: absolute;
        margin: -1.1rem -3rem 0;
    }
    .pn_review_profile span {
        position: absolute;
        padding: 1rem;
    }
    .pn_review_rating img {
        width: auto;
    }
}
</style>