<script>
import { carousel_data } from "../data/carouselData"
export default {
    methods: {
        isActive(index) {
            return index === this.currentIndex
        },
        nextSlide() {
            this.currentIndex = (this.currentIndex + 1) % this.carousel_data.length;
        },
        prevSlide() {
          this.currentIndex = (this.currentIndex - 1 + this.carousel_data.length) % this.carousel_data.length;
        },
        getCircleStyle(percentage) {
            return {
        '--percentage': `${percentage}`,
      };
    },
    },
    data() {
        return {
            carousel_data,
            currentIndex: 0,
            rates: [
                { label: 'PASS RATE', value: 95 },
                { label: 'REFERRAL RATE', value: 100 },
                { label: 'ACCIDENT RATE', value: 0 }
            ]
        }
    }
}

</script>

<template>

    <div id="bg_jumbo_container">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="overlay_text pt-">
                        <h1>Drive with Avada</h1>
                        <span>We offer the finest driving tuition money can buy</span>
                    </div>
                </div>
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
    <div id="courses_rate_container">
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
                                <img src="../assets/images/courses-passplus.jpg" alt="courses_passplus">
                                <h5 class="mt-3">Pass Plus</h5>
                                <button>LEARN MORE</button>
                            </div>
                            <div class="text-center">
                                <img src="../assets/images/course-intensive.jpg" alt="course_intensive">
                                <h5 class="mt-3">Intensive Course</h5>
                                <button>LEARN MORE</button>
                            </div>
                            <div class="text-center">
                                <img src="../assets/images/courses-instructor.jpg" alt="courses_instructor">
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
                    <div class="rate_card" v-for="rate, index in rates" :key="index">
                    <span class="grey_circle">
                        <span class="green_circle" :style="getCircleStyle(rate.value)">
                        <span class="percentage">{{ rate.value }}%</span>
                        </span>
                    </span>
                    <h6>{{ rate.label }}</h6>
                    </div>
                </div>
                </div>
            </div>
        </div>
        <div class="position-relative">
            <div id="triangle_bottom_container">
            </div>
        </div>
        
    </div>
    <div id="instructors_container">
        <div class="my_container">
            <div class="d-flex mb-4">
                <div class="col-12">
                    <h1>Your Instructors</h1>
                </div>
            </div>
            <div class="d-flex">
                <div class="col-8">
                    <span>Lorem ipsum dolor sit, amet consectetur adipisicing elit. 
                        Doloremque quia animi cum quasi aperiam! Neque consectetur perspiciatis non velit. 
                        Ex omnis esse vel.
                    </span>
                </div>
                <div class="col-4">
                    <button>MORE ABOUT US</button>
                </div>
            </div>
            <div id="instructors_cards_container">
                <div class="my_container">
                    <div class="d-flex justify-content-between">
                        <div class="instructor_card">
                            <div class="mini_size">
                                <img src="../assets/images/instructor-mikehart.jpg"  title="instructor-mikehart">
                            </div>
                            <h5>Mike Hart</h5>
                            <div>
                                <i class="bi bi-facebook"></i>
                                <i class="bi bi-twitter mx-3"></i>
                                <i class="bi bi-instagram"></i>
                            </div>
                            <span>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</span>
                        </div>
                        <div class="instructor_card">
                            <div class="mini_size">
                                <img src="../assets/images/instructor-johnsmith.jpg"  title="instructor-johnsmith">
                            </div>
                            <h5>John Smith</h5>
                            <div>
                                <i class="bi bi-facebook"></i>
                                <i class="bi bi-twitter mx-3"></i>
                                <i class="bi bi-instagram"></i>
                            </div>
                            <span>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</span>
                        </div>
                        <div class="instructor_card">
                            <div class="mini_size">
                                <img src="../assets/images/instructor-angelahart.jpg"  title="instructor-angelahart">
                            </div>
                            <h5>Angela Hart</h5>
                            <div>
                                <i class="bi bi-facebook"></i>
                                <i class="bi bi-twitter mx-3"></i>
                                <i class="bi bi-instagram"></i>
                            </div>
                            <span>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</span>
                        </div>
                    </div>
                </div>
            </div>
            
        </div>
    </div>
    <div id="testimonials_container">
        <div class="pt-5">
            <h1 class="text-center">Testimonials</h1>
            <span class="d-block text-center mb-4">Here's what our happy drivers had to say about our services</span>
        </div>
        <div class="carousel_container">
            <div id="carouselExampleIndicators" class="carousel slide p-100" data-bs-ride="carousel" data-bs-interval="4000">
                <div class="carousel-indicators">
                  <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                  <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
                  <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
                  <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3" aria-label="Slide 4"></button>
                  <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="4" aria-label="Slide 5"></button>
                </div>
                <div class="carousel-inner">
                    <div v-for="slide, index in carousel_data" :key="index" class="carousel-item" :class="{'active' : isActive(index)}">
                        <div class="d-flex flex-column align-items-center">
                            <div class="mini_size">
                                <img :src="slide.img" class="d-block w-100" :alt="slide.name">
                            </div>
                            <div class="text-center text_content">
                                <span class="d-block fst-italic mb-4">{{ slide.text }}</span>
                                <span class="fw-semibold">{{ slide.name }}</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div id="latest_news_container">
        <div class="my_container">
            <div class="latest_news_card text-center">
                <h1>Latest News</h1>
                <div class="container">
                    <div class="row">
                        <div class="col-6">
                            <div class="pt-4">
                                <div class="img_resize">
                                    <img src="../assets/images/blog-choosecar-700x441.jpg" alt="">
                                </div>
                                <div class="text_content">
                                    <h4 class="green_text m-0">What Car to Start With?</h4>
                                    <span>February 7th, 2019 | <span class="green_text">0 comments</span></span>
                                    <p class="mt-3">Lorem ipsum dolor sit amet, consectetur adpiscing</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-6">
                            <div class="pt-4">
                                <div class="img_resize">
                                    <img src="../assets/images/blogpost-10and2-700x441.jpg" alt="">
                                </div>
                                <div class="text_content">
                                    <h4 class="green_text m-0">Avada Driving School Expanding</h4>
                                    <span>February 7th, 2019 | <span class="green_text">0 comments</span></span>
                                    <p class="mt-3">Lorem ipsum dolor sit amet, consectetur adpiscing</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-12 d-flex justify-content-center mt-5">
                            <button>MORE FROM THE BLOG</button>
                        </div>
                    </div>
                </div>

            </div>
            <div class="news_bottom"></div>
        </div>
    </div>
    <div id="newsletter_container">
        <div class="container">
            <div class="row justify-content-center text-center">
                <div class="col-12 w-50 d-flex flex-column justify-content-center text-center">
                    <h1>Sign up to our Newsletter</h1>
                    <input type="email">
                    <button type="submit">SUBSCRIBE</button>
                </div>
                <p class="mt-4">(We do not share your data with anybody, and only use it for intended purpose)</p>
            </div>
        </div>

    </div>

</template>

<style scoped>

#bg_jumbo_container {
    background-image: url("../assets/images/homepage-hero-background.jpg");
    background-size: cover;
    background-position: center;
    
    .container {
        padding: 250px 0;
        
        .overlay_text {
            color: #ffffff;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);

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

                    &:hover {
                        background-color: #6fb161;
                    }
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

#courses_rate_container {
    height: 800px;

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
                top: 0;
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

                    &:hover {
                        background-color: #6fb161;
                    }
                }
            }
        }

        #rate_cards_container {

            .my_container {
                width: 1200px;
                height: 135px;
                margin: 0 auto;

                .rate_card {
                    text-align: center;
                    z-index: 3;
                    top: 20px;
                    width: calc(100% / 3 - 5px);
                    height: 370px;
                    background-color: white;
                    border-radius: 8px;
                    box-shadow: 0px 20px 20px rgba(0, 0, 0, 0.233);
                    border-top: 6px solid #7ABC64;

                    .grey_circle {
                        position: relative;
                        display: inline-flex;
                        justify-content: center;
                        align-items: center;
                        margin-top: 158px;
                        color: grey;
                        
                        .green_circle {
                            position: absolute;
                            width: 180px;
                            height: 180px;
                            border-radius: 50%;
                            font-size: 46px;
                            line-height: 144px;
                            text-align: center;
                            background: white;
                            border: 8px solid transparent;
                            background-clip: padding-box;
                            z-index: 1;
                        }
                        .green_circle::before {
                            content: '';
                            position: absolute;
                            top: -4px;
                            left: 0;
                            width: 100%;
                            height: 100%;
                            border-radius: 50%;
                            background: conic-gradient(#7abc64 calc(var(--percentage) * 1%), rgb(197, 197, 197) 0);
                            mask: radial-gradient(farthest-side, transparent calc(100% - 8px), rgb(230, 230, 230) calc(100% - 8px));
                            -webkit-mask: radial-gradient(farthest-side, transparent calc(100% - 8px), rgb(197, 197, 197) calc(100% - 8px));
                            z-index: -1;
                        }

                        .percentage {
                            z-index: 2;
                            margin-top: 10px;
                            position: relative;
                            color: grey;
                        }
                    }

                    h6 {
                        margin-top: 100px;
                        color: grey;
                    }
                }
            }
        }

        #courses_options {
            color: #7799AD;

            img {
                width: 180px ;
                height: 180px ;
            }

            button {
                font-size: 10px;
                font-weight: 600;
                padding: 8px 25px;
                border: 3px solid #7799AD;
                border-radius: 25px;
                cursor: pointer;
                color: #7799AD;

                &:hover {
                    color: #7ABC64;
                    border: 3px solid #7ABC64;
                }
            }
        }
    }

    #triangle_bottom_container {
        position: absolute;
        top: -2px;
        width: 100%;
        height: 135px;
        background-image: url("../assets/images/latestnews-bottom.png");
        filter: brightness(0) saturate(100%) invert(98%) sepia(3%) saturate(724%) hue-rotate(175deg) brightness(95%) contrast(96%);;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center bottom;
    }

}

#instructors_container {
    padding-top: 60px;
    height: 670px;

    span {
        font-size: 18px;
        line-height: 38px;
    }

    .my_container {
        width: 1200px;
        height: 380px;
        margin: 0 auto;
        position: relative;

        button {
            float: right;
            width: 90%;
            font-size: 14px;
            font-weight: 700;
            background-color: #7ABC64;
            color: #ffffff;
            padding: 8px 65px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            transition: background-color 0.3s ease;

            &:hover {
                background-color: #6fb161;
            }
        }

        #instructors_cards_container {
            position: absolute;
            bottom: 0;

            .my_container {
                width: 1200px;
                height: 135px;
                margin: 0 auto;

                .instructor_card:nth-child(2) {
                    height: 440px;

                    .mini_size {
                        height: 190px;
                    }
                }

                .instructor_card {
                    text-align: center;
                    display: inline-flex;
                    flex-direction: column;
                    align-items: center;
                    z-index: 3;
                    top: 20px;
                    width: calc(100% / 3 - 5px);
                    height: 430px;
                    background-color: white;
                    border-radius: 8px;
                    box-shadow: 0px 20px 20px rgba(0, 0, 0, 0.233);
                    border-top: 6px solid #7ABC64;
                    color: grey;

                    .mini_size {
                        width: 300px;
                        height: 170px;
                        margin-top: 40px;

                        img {
                            width: 100%;
                            height: 100%;
                            object-fit: cover;
                            object-position: center;

                            &:hover {
                                box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.308);
                            }
                        }
                    }
                
                    h5 {
                        margin-top: 35px;
                        color: black;
                    }

                    span {
                        padding: 0 27px;
                        font-size: 15px;
                    }
                }
            }
        }
    }
}

#testimonials_container {
    background-image: url("../assets/images/testimonial-background.jpg");
    height: 720px;
    background-size: cover;
    color: grey;

    h1 {
        color: rgb(87, 87, 87);
        margin-top: 90px;
    }

    h6 {
        padding: 0 450px;
    }

    .p-100 {
        padding: 0 70px 50px 70px;
    }

    .carousel-indicators {

        button {
            width: 8px;
            height: 8px;
            border-radius: 50%;
            background-color: rgba(128, 128, 128, 0);
            border: 2px solid grey;
        }

        .active {
            background-color: grey;
        }
    
    }

    .carousel-inner {
        display: flex;
        justify-content: space-between;

        .text_content {
            padding: 0 450px;
        }

        .carousel-item {
          display: none;
        }

        .carousel-item.active {
          display: block;
        }
    }

    .mini_size {
        width: 140px;
        height: 140px;
        border-radius: 50%;
        margin-top: 20px;
        margin-bottom: 30px;
    }
}

#latest_news_container {
    background-image: url("../assets/images/latestnews-background.jpg");
    height: 750px;
    background-size: cover;
    padding-top: 80px;
    background-position: bottom;

    .green_text {
        color:#7ABC64;
    }

    .my_container {
        width: 1200px;
        height: 635px;
        margin: 0 auto;
        position: relative;

        .latest_news_card {
            width: 100%;
            height: 100%;
            position: absolute;
            top: -120px;
            border-top: 6px solid #7799AD;
            border-top-left-radius: 6px;
            border-top-right-radius: 6px;
            background-color: white;
            padding-top: 30px;

            .img_resize {
                width: 540px;
                height: 300px;
                margin: 0 auto;

                img {
                    width: 100%;
                    height: 100%;
                    object-fit: cover;
                    object-position: center;
                }
            }

            .text_content {
                margin-top: 20px;
                color: grey;

                span {
                    font-size: 12px;
                }
            }

            button {
                font-size: 14px;
                font-weight: 700;
                background-color: #7ABC64;
                color: #ffffff;
                padding: 8px 25px;
                border: none;
                border-radius: 25px;
                cursor: pointer;
                transition: background-color 0.3s ease;

                &:hover {
                    background-color: #6fb161;
                }
            }
        }

        .news_bottom {
            background-image: url("../assets/images/latestnews-bottom-1200x105.png");
            width: 100%;
            height: 150px;
            background-size: contain;
            background-repeat: no-repeat;
            position: absolute;
            bottom: -30px;
        }
    }
}

#newsletter_container {
    background-image: url("../assets/images/newsletter_background.jpg");
    height: 380px;
    background-size: cover;

    .container {
        padding-top: 50px;

        input {
            margin-top: 40px;
            border-radius: 5px;
            padding: 10px 20px;
            font-size: 16px;
            border: 1px solid rgb(223, 223, 223);
        }

        button {
            margin-top: 30px;
            font-size: 14px;
            font-weight: 700;
            background-color: #7ABC64;
            color: #ffffff;
            padding: 10px 25px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            transition: background-color 0.3s ease;

            &:hover {
                background-color: #6fb161;
            }
        }

        p {
            color: grey;
        }
    }
}

</style>
