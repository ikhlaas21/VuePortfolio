<template>
    <div class="projects">

       
        <body>
            <div class="container">
                
                    <div class="col-sm-4">
                        <div class="card">
                            <div class="img-box">
                                <img
                                    src="https://images.unsplash.com/photo-1432251407527-504a6b4174a2?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&auto=format&fit=crop&w=1400&q=80" />
                            </div>
                            <div class="content">
                                <h2>Card One</h2>
                                <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod
                                    tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero
                                    eos et accusam et justo duo dolores et ea rebum.</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-4">
                        <div class="card">
                            <div class="img-box">
                                <img
                                    src="https://images.unsplash.com/photo-1569776277464-9dc1113d1242?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&auto=format&fit=crop&w=1400&q=80" />
                            </div>
                            <div class="content">
                                <h2>Card Two</h2>
                                <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod
                                    tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero
                                    eos et accusam et justo duo dolores et ea rebum. </p>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-4">
                        <div class="card">
                            <div class="img-box">
                                <img
                                    src="https://images.unsplash.com/photo-1570030990547-f6b13f3062ff?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1400&q=80" />
                            </div>
                            <div class="content">
                                <h2>Card Three</h2>
                                <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod
                                    tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero
                                    eos et accusam et justo duo dolores et ea rebum.</p>
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

 .card {
    position: relative;
    background-color: maroon;
    margin: 30px 10px;
    padding: 20px 15px;
    max-width: 300px;
    height: 215px;
    display: flex;
    flex-direction: column;

    transition: 300ms ease-in-out;

}

 .card:hover {
    height: 420px;
    cursor: pointer;
}

 .card .img-box {
    position: relative;
    width: 260px;
    height: 260px;
    top: -60px;
    left: 20px;

    z-index: 1;
}

 .card .img-box img {
    width: 225px;
    border-radius: 4px;

}

 .card .content {
    position: relative;
    margin-top: -140px;
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
    margin-top: -60px;
    transition-delay: 300ms;
}
@media (max-width: 321px) {
    .col-sm-4{
width: 540px;
padding-left: 110px;

    }
    .container{
        margin-top: 480px;
    }
    .card{
        min-width: 200px;
    }
}
</style>