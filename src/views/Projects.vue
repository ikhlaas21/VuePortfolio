<template>
    <div class="projects">

        <body>
            <div id="con1" class="container">
               
                                    
                    <div class="col-sm-4 ">
                        <div class="card">
                            <div class="img-box">
                                <img
                                    src="https://i.postimg.cc/WzCdJgTg/calculator-2022-07-22-113319.jpg" />
                            </div>
                            <div class="content">
                                <h2>My Calculator</h2>
                                <p>This Project is a functional calculator that I designed. It was Coded using HTML, CSS, JavaScript</p>
                                <a href="https://github.com/ikhlaas21/WorkingCalculator"><i class="bi bi-github"></i></a>
                                <a href="https://ikhlaascalculator.netlify.app"><i class="bi bi-link"></i></a>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-4">
                        <div class="card">
                            <div class="img-box">
                                <img
                                    src="https://i.postimg.cc/qvZfTwBk/charizard.jpg" />
                            </div>
                            <div class="content">
                                <h2>3D Printing</h2>
                                <p>This image is of my 3D printed Charizard. I have recently started a 3D Printing business which is an ongoing Project. My plan is to create my own Website to list my products. </p>
                                <a href="https://www.instagram.com/rnrcustom3dprints/"><i class="bi bi-instagram"></i></a>
                                
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-4">
                        <div class="card">
                            <div class="img-box">
                                <img
                                    src="https://i.postimg.cc/X7hFkqT5/Screenshot-2022-07-22-115544.jpg" />
                            </div>
                            <div class="content">
                                <h2>Properties</h2>
                                <p>This Project is a property listing site. It was coded using HTML, CSS, Bootstrap, JavaScript</p>
                                <a href="https://github.com/ikhlaas21/Properties"><i class="bi bi-github"></i></a>
                                <a href="https://homify-ikhlaas.netlify.app"><i class="bi bi-link"></i></a>
                            </div>
                        </div>

            

            </div>
            </div>
           <div id="con2" class="container">
               
                                    
                    <div class="col-sm-4 ">
                        <div class="card">
                            <div class="img-box">
                                <img
                                    src="https://i.postimg.cc/WzCdJgTg/calculator-2022-07-22-113319.jpg" />
                            </div>
                            <div class="content">
                                <h2>My Calculator</h2>
                                <p>This Project is a functional calculator that I designed. It was Coded using HTML, CSS, JavaScript</p>
                                <a href="https://github.com/ikhlaas21/WorkingCalculator"><i class="bi bi-github"></i></a>
                                <a href="https://ikhlaascalculator.netlify.app"><i class="bi bi-link"></i></a>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-4">
                        <div class="card">
                            <div class="img-box">
                                <img
                                    src="https://i.postimg.cc/qvZfTwBk/charizard.jpg" />
                            </div>
                            <div class="content">
                                <h2>3D Printing</h2>
                                <p>This image is of my 3D printed Charizard. I have recently started a 3D Printing business which is an ongoing Project. My plan is to create my own Website to list my products. </p>
                                <a href="https://www.instagram.com/rnrcustom3dprints/"><i class="bi bi-instagram"></i></a>
                                
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-4">
                        <div class="card">
                            <div class="img-box">
                                <img
                                    src="https://i.postimg.cc/X7hFkqT5/Screenshot-2022-07-22-115544.jpg" />
                            </div>
                            <div class="content">
                                <h2>Properties</h2>
                                <p>This Project is a property listing site. It was coded using HTML, CSS, Bootstrap, JavaScript</p>
                                <a href="https://github.com/ikhlaas21/Properties"><i class="bi bi-github"></i></a>
                                <a href="https://homify-ikhlaas.netlify.app"><i class="bi bi-link"></i></a>
                            </div>
                        </div>

            

            </div>
            </div>
           
        </body>
    </div>


</template>

<script>


export default {

}

</script>
<style scoped>
/* .tap{
    position: fixed;
    top:80%;
    left:50%;
    width: 150px;
    height: 100px;
    background-color: blue;

} */
i{
    font-size: 30px;
    color:rgb(253, 216, 141)  ;
    padding: 5px;
}

body {
    background-color: #2D3A3D;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 50px;
}
.container {
    position: relative;
    width: 1000px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    padding: 30px;
   
}
 #con1 {
   
    margin-top: 50px;
}
/* .con2 {
   
    width: 1000px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    /* padding-top: -500px;
} */

.card {
    position: relative;
    background-color: maroon;
    margin: 30px 10px;
    padding: 20px 15px;
    max-width: 300px;
    height: 240px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;

    transition: 300ms ease-in-out;

}

.card:hover {
    /* height: 420px; */
    cursor: pointer;
   background-color:rgba(128, 0, 0, 0.438);
   
 
    
}

.card .img-box {
    position: relative;
    width: 260px;
    height: 260px;
    top: -60px;
    left: 20px;

    z-index: 1;
}
img{
    transition: 300ms ease-in-out;
}
img:hover{
    opacity: 0;

}

.card .img-box img {
    width: 225px;
    height: 225px;
    scale: 1;
    border-radius: 10px;
    object-fit: cover;


}

.card .content {
    position: relative;
    margin-top: -240px;
    padding: 10px 15px;
    text-align: center;
    color: rgb(253, 216, 141);
    visibility: hidden;
    opacity: 0;
    transition: 300ms ease-in-out;
}

.card:hover .content {
    visibility: visible;
    opacity: 1;
    /* padding-bottom: 560px; */
    transition-delay: 300ms;
    /* z-index: 50; */
}

@media (max-width: 321px) {
    .col-sm-4 {
        width: 540px;
        padding-left: 110px;

    }

    #con1 {
        margin-top:1500px;
    }

    .card {
        min-width: 200px;
    }
}
@media (max-width: 426px) {
    .col-sm-4 {
        width: 540px;
        padding-left: 110px;

    }

    #con1 {
        margin-top:1500px;
    }

    .card {
        min-width: 200px;
    }
}
</style>