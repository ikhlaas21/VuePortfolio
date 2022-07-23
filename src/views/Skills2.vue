<template>
    <main>

        <div class="container">
            <div class="row row-cols-1 row-cols-md-3 g-4 ">
                <div class="col">
                    <div class="card h-100">
                        <img src="https://i.postimg.cc/x1FmZVQz/webdev.jpg" class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">Web Development</h5>
                            <p class="card-text">Web development refers to the building, creating, and
                                maintaining
                                of websites. It includes aspects such as web design, web publishing, web programming,
                                and database
                                management. It is the creation of an application that works over the internet i.e.
                                websites.</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card h-100">
                        <img src="https://i.postimg.cc/XvGsHgRn/web-design-blogs-to-follow-featured-image.jpg"
                            class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">Web Design</h5>
                            <p class="card-text">Web design refers to the design of websites that are displayed
                                on
                                the internet. It usually refers to the user experience aspects of website development
                                rather than
                                software development.</p>

                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card h-100">
                        <img src="https://i.postimg.cc/R040GP6H/rnrgif.gif" class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">3D Printing</h5>
                            <p class="card-text">Three-dimensional (3D) printing is an additive manufacturing
                                process that creates a physical object from a digital design. The process works by
                                laying down thin
                                layers of material in the form of liquid or powdered plastic, metal or cement, and then
                                fusing the
                                layers together..</p>
                        </div>
                    </div>
                </div>
            </div>
           <br>
                <router-link to="/skills">
                    <button class="text-center mx-auto">Go Back</button>
                </router-link>
           
        


        </div>
    </main>
</template>

<script>
export default {

}
</script>

<style scoped>
.container {
    margin-top: -10px;
}

button {

    background-color: rgb(253, 216, 141);
    width: 90px;
    color: #222;
    border: solid 3px maroon;
    border-radius: 3px;
    transition: 0.5s;



}

button:hover {
    color: maroon;
    border: solid 3px rgb(253, 216, 141);
    border-radius: 3px rgb(253, 216, 141);
    background-color: rgb(253, 216, 141);
    transform: translateX(10px);
}

.card img {
    aspect-ratio: 1;
    height: 270px;
    object-fit: cover;
}

.card {
    border-color: maroon;
    border-width: 5px;
    background-color: rgb(253, 216, 141);
    width: 310px;



}

h5 {
    transition: 0.5s;
}

h5:hover {
    color: maroon;
    /* border: solid 3px rgb(253, 216, 141);
    border-radius: 3px rgb(253, 216, 141); */
    background-color: rgb(253, 216, 141);
    transform: translateX(10px);
}
@media (max-width: 321px) {
    .container{
        
        padding-bottom: 20px;
        margin-top: 1200px;
        
       
    }}
    .card{
        width: 270px;
        margin-left: 15px;
    }
    button{
        margin-left: 30px;
    }
@media (max-width: 426px) {
    .container{
        
        padding-bottom: 20px;
        margin-top: 1200px;
        
       
    }}
    .card{
        width: 270px;
        margin-left: 15px;
    }
    button{
        margin-left: 30px;
    }
</style>