<template>
    <div class="testimonials2">

        <section class="pn_reviews mt-5 ">
            <div class="container">
                <div class="row">
                    <div class="col-sm-12">
                        <h1 class="text-center ">Testimonials</h1>
                    </div>

                    <div class="col-sm-12 col-lg-4">
                        <div class="pn_testimonial_box ">
                            <p class="text-justify">What does Lorem Ipsum mean? Derived from Latin dolorem ipsum (“pain
                                itself”), Lorem Ipsum is filler text used by publishers and graphic designers used to
                                demonstrate graphic elements.
                            </p>

                            <div class="row pt-3">
                                <div class="col-sm-6 pn_review_profile"><img
                                        src="https://desklib.com/static/src/assets/images/v2/profile_1.svg"
                                        class="border-radius-12 float-right" alt="client image" /> <span> Charles Boyle
                                    </span> </div>

                            </div>
                        </div>
                    </div>
                    <div class="col-sm-12 col-lg-4">
                        <div class="pn_testimonial_box mt-4">
                            <p class="text-justify">What does Lorem Ipsum mean? Derived from Latin dolorem ipsum (“pain
                                itself”), Lorem Ipsum is filler text used by publishers and graphic designers used to
                                demonstrate graphic elements.
                            </p>
                            <div class="row pt-3">
                                <div class="col-sm-6 pn_review_profile"><img
                                        src="https://desklib.com/static/src/assets/images/v2/profile_2.svg"
                                        class="border-radius-12 float-right" alt="client image" /> <span> Gina Lannety
                                    </span> </div>

                            </div>
                        </div>
                    </div>
                    <div class="col-sm-12 col-lg-4">
                        <div class="pn_testimonial_box mt-4">
                            <p class="text-justify">What does Lorem Ipsum mean? Derived from Latin dolorem ipsum (“pain
                                itself”), Lorem Ipsum is filler text used by publishers and graphic designers used to
                                demonstrate graphic elements.
                            </p>
                            <div class="row pt-3">
                                <div class="col-sm-6 pn_review_profile"><img
                                        src="https://desklib.com/static/src/assets/images/v2/profile_3.svg"
                                        class="border-radius-12 float-right" alt="client image" /> <span> Dug Judey
                                    </span> </div>

                            </div>
                        </div>
                    </div>
                </div>
                <br>
                
            </div>
                 <router-link to="testimonials"><button>Go Back</button></router-link>
        </section>
    </div>

</template>

<script>
export default {

}
</script>

<style scoped>

span{
font-weight: bold;

}
button{
    background-color:rgb(253, 216, 141);
    width: 95px;
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
.container {
    width: 900px;
    margin-top: -50px;
}

.pn_testimonial_box {
    font-weight: 300;
    padding: 2rem;
    margin: 2rem;
    border: 5px solid maroon;
    position: relative;
    transition: 1s;
    transform: scale(0.9);
    background-color: rgb(253, 216, 141);
    -webkit-border-radius: 4rem;
    -moz-border-radius: 4rem;
    -ms-border-radius: 4rem;
    border-radius: 4rem;
}

.pn_testimonial_box:hover {
    /* box-shadow: 2px 4px 8px #d6d8da; */
    border: 5px solid rgb(253, 216, 141);
    /* transform: scale(0.95); */
    position: relative;
    z-index: 1;
}



.pn_review_profile img {
    position: absolute;
    margin: -1rem -5rem 0;
    transition: 0.9s;
}
.pn_review_profile img:hover {
    transform: rotate(360deg);
}

.pn_review_profile span {
    position: absolute;
}


@media (max-width: 321px) {
    span{
    padding-left: 35px;
}
    .container {
        width: 250px;
        margin-top: 900px;

    }

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
        border: 5px solid maroon;
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
    .pn_review_profile{
        padding-bottom: 19px;
    }

    
}
</style>