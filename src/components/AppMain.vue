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
                    <div class="mt-5">
                        <h1>Get Behind The Wheel</h1>
                        <div class="pe-5">
                            <span class="d-block pe-5 mb-4 lh-lg fw-semibold">Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa adipisci ea, 
                                doloribus libero voluptates cupiditate. Culpa adipisci ea, 
                                doloribus libero voluptates cupiditate
                            </span>
                            <span class="d-block pe-5 fw-semibold lh-lg fs-13">Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa adipisci ea, 
                                doloribus libero voluptates cupiditate est obcaecati repudiandae consequuntur 
                                cumque ab blanditiis dolorem eius rem quibusdam sunt ipsa soluta numquam. Obcaecati repudiandae consequuntur 
                                cumque ab blanditiis dolorem eius rem quibusdam sunt ipsa soluta numquam.
                            </span>
                        </div>
                    </div>
                </div>
                <div class="col-6 position-relative">
                    <div class="my_card text-center">
                        <h4>First Lesson Free!</h4>
                        <span>When you make a block booking with us your first lesson is included free</span>
                        <div class="form_control">
                            <div class="d-flex mb-3">
                                <input class="my_form" type="text" placeholder="Your name*">
                                <div class="mini_size">
                                    <img src="../assets/images/image.png" alt="">
                                </div>
                            </div>
                            <input class="my_form mb-4" type="email" name="email" id="" placeholder="Email*">
                            <input class="my_form mb-4" type="number" name="Telephone" id="" placeholder="Telephone">
                            <input class="my_form mb-4" type="text" placeholder="Location">
                            <button type="submit">REQUEST A CALLBACK</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div id="start_learning_container">
        <div class="my_container">
            <div class="content">
                <div class="d-flex justify-content-between align-items-center">
                    <div class="left_content">
                        <h1>Start Learning to Drive Today</h1>
                        <span>Give us a call to schedule your first driving lesson</span>
                    </div>
                    <div class="right_content">
                        <i class="bi bi-telephone-fill"></i>
                        <span class="me-5"> 1-800-555-555</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div id="courses_instructors_container">
        <div id="courses_container">
            <div class="my_container">
                <div class="row">
                    <div class="col-4 position-relative">
                        <div class="courses_info_card">
                            <div class="mini_size">
                                <img src="../assets/images/new-corner.jpg" alt="">
                            </div>
                            <div class="content">
                                <h2 class="mt-4">Courses</h2>
                                <span class="d-block my-3">Lorem ipsum dolor sit, amet consectetur adipisicing elit. 
                                    Accusamus tempore laborum quae aliquid! Doloremque nemo debitis delectus ea eveniet hic numquam nihil minima.
                                </span>
                                <button>COURSE INFORMATION</button>
                            </div>

                        </div>
                    </div>
                    <div class="col-8">
                        <div id="courses_options" class="d-flex justify-content-evenly mt-5">
                            <div class="text-center">
                                <img src="../assets/images/courses-passplus.jpg" alt="">
                                <h5 class="mt-3">Pass Plus</h5>
                                <button>LEARN MORE</button>
                            </div>
                            <div class="text-center">
                                <img src="../assets/images/course-intensive.jpg" alt="">
                                <h5 class="mt-3">Intensive Course</h5>
                                <button>LEARN MORE</button>
                            </div>
                            <div class="text-center">
                                <img src="../assets/images/courses-instructor.jpg" alt="">
                                <h5 class="mt-3">Instructors</h5>
                                <button>LEARN MORE</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div id="rate_cards_container">
                <div class="my_container">
                    <div class="d-flex justify-content-between position-relative">
                        <div class="rate_card">
                            <span>95%</span>
                            <h6>PASS RATE</h6>
                        </div>
                        <div class="rate_card">
                            <span>100%</span>
                            <h6>REFERRAL RATE</h6>
                        </div>
                        <div class="rate_card">
                            <span>0%</span>
                            <h6>ACCIDENT RATE</h6>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div id="triangle_bottom_container">
        </div>
    </div>
  
</template>

<style scoped>

#bg_jumbo_container {
    background-image: url("../assets/images/homepage-hero-background.jpg");
    height: 600px;
    background-size: cover;
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
            top: -55px;
            right: 12px;
            width: 500px;
            height: 480px;
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.1);
            padding: 20px;
            margin-top: 20px;

            h4 {
                color: #7ABC64;
                margin: 20px 0;
            }

            span {
                font-size: 12px;
            }

            .form_control {
                position: relative;
                margin-top: 30px;

                .my_form {
                    font-size: 10px;
                    padding: 10px;
                    width: 100%;
                    border-radius: 3px;
                    border: 1px solid #cccccc;
                    background-color: #f2f2f2;
                    margin-bottom: 10px;
                }

                .mini_size {
                    width: 20px;
                    height: 30px;
                    position: absolute;
                    top: 5px;
                    right: 0;

                    img {
                        object-fit: cover;
                        right: 10px;
                        width: 50%;
                        height: 50%;
                        cursor: pointer;
                    }
                }

                button {
                    font-size: 10px;
                    font-weight: 700;
                    background-color: #7ABC64;
                    color: #ffffff;
                    padding: 8px 25px;
                    border: none;
                    border-radius: 25px;
                    cursor: pointer;
                    transition: background-color 0.3s ease;
                }
            }
        }
    }
}

#start_learning_container {
    background-image: url("../assets/images/horizontal-cta-background.jpg");
    height: 250px;
    background-size: cover;
    background-position: center;


    .my_container {
        width: 1200px;
        height: 250px;
        margin: 0 auto;

        .content {
            padding-top: 100px;
            color: white;

            .left_content {
                span {
                    font-size: 20px;

                }
            }

            .right_content {
                font-size: 30px;
            }
        }
    }
}

#courses_instructors_container {
    height: 1000px;

    #courses_container {
        background-image: url("../assets/images/promise-background.jpg");
        height: 400px;
        background-size: cover;
        background-position: bottom;

        .my_container {
            width: 1200px;
            height: 400px;
            margin: 0 auto;
        }

        .courses_info_card {
            position: absolute;
            top: -25px;
            width: 95%;
            height: 350px;
            background-color: white;
            border-radius: 5px;
            box-shadow: 0px 20px 20px rgba(0, 0, 0, 0.233);

            .mini_size {
                width: 80px;
                height: 80px;
                position: absolute;
                top: 0px;
                left: 0;

                img {
                    width: 100%;
                    height: 100%;
                    border-top-left-radius: 5px;
                }
            }
            
            .content {
                text-align: center;
                padding: 20px;
                span {
                    padding: 20px;
                    font-size: 14px;
                    line-height: 25px;
                }

                button {
                    font-size: 10px;
                    font-weight: 700;
                    background-color: #7ABC64;
                    color: #ffffff;
                    padding: 8px 25px;
                    border: none;
                    border-radius: 25px;
                    cursor: pointer;
                    transition: background-color 0.3s ease;
                }
            }
        }

        #rate_cards_container {

            .my_container {
                width: 1200px;
                height: 135px;
                margin: 0 auto;

                .rate_card {
                    position: absolute;
                    top: 20px;
                    width: calc(100% / 3);
                    height: 350px;
                    background-color: white;
                    border-radius: 5px;
                    box-shadow: 0px 20px 20px rgba(0, 0, 0, 0.233);
                }
            }
        }

        #courses_options {
            color: rgb(63, 63, 66);

            img {
                width: 180px ;
                height: 180px ;
            }

            button {
                font-size: 10px;
                font-weight: 600;
                padding: 8px 25px;
                border: 3px solid rgb(63, 63, 66);
                border-radius: 25px;
                cursor: pointer;
            }
        }
    }

    #triangle_bottom_container {
        width: 100%;
        height: 135px;
        background-color: #6b72721c;
        background-image: url("../assets/images/latestnews-bottom.png");
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center bottom;
    }
}

</style>
