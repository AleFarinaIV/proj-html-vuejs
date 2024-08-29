<script>
export default {
    
}

</script>

<template>

    <div id="bg_jumbo_container">
        <div class="my_container">
            <div class="overlay_text">
                <h1>Drive with Avada</h1>
                <span>We offer the finest driving tuition money can buy</span>
            </div>
        </div>
    </div>
    <div id="form_container">
        <div class="my_container">
            <div class="row">
                <div class="col-6">
                    <h1>Get Behind The Wheel</h1>
                    <div class="pe-5">
                        <span class="d-block pe-5 mb-4 lh-lg fw-semibold">Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa adipisci ea, 
                            doloribus libero voluptates cupiditate. Culpa adipisci ea, 
                            doloribus libero voluptates cupiditate
                        </span>
                        <span class="d-block pe-5 fw-semibold fs-13">Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa adipisci ea, 
                            doloribus libero voluptates cupiditate est obcaecati repudiandae consequuntur 
                            cumque ab blanditiis dolorem eius rem quibusdam sunt ipsa soluta numquam. Obcaecati repudiandae consequuntur 
                            cumque ab blanditiis dolorem eius rem quibusdam sunt ipsa soluta numquam.
                        </span>
                    </div>
                </div>
                <div class="col-6 position-relative">
                    <div class="my_card text-center">
                        <h4>First Lesson Free!</h4>
                        <span>When you make a block booking with us your first lesson is included free</span>
                    </div>

                </div>
            </div>
        </div>
    </div>
  
</template>

<style scoped>

#bg_jumbo_container {
    background-image: url("../assets/images/homepage-hero-background.jpg");
    height: 600px;
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
    
    .my_container {
        width: 1200px;
        height: 500px;
        margin: 0 auto;
        position: relative;
        
        .overlay_text {
            position: absolute;
            top: 50%;
            left: 0;
            color: #ffffff;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            z-index: 100;

            h1 {
                font-size: 56px;
            }
            
            span {
                font-size: 24px;
            }
     
        }
    }

}

#form_container {

    .my_container {
        width: 1200px;
        height: 500px;
        margin: 0 auto;

        span {
            color: grey;
        }

        .fs-13 {
            font-size: 13px;
        }

        .my_card {
            position: absolute;
            top: -100px;
            width: 400px;
            height: 500px;
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.1);
            padding: 20px;
            margin-top: 20px;
        }
    }
}

</style>
