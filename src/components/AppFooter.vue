<script>
export default {

}
</script>

<template>

    <div id="top_footer" class="py-5">
        <div class="container">
            <div class="row">
                <div class="col-3">
                    <div>
                        <img src="../assets/images/avada-drivers-logo-2x-200x39.png" alt="">
                    </div>
                    <p>Avada Driving School is the right choice for experienced drivers looking for a refresher course, or the brand new driver wanting to pass first time.</p>
                </div>
                <div class="col-3">
                    <ul class="text-secondary">
                        <h6 class="text-white mb-4">CONTACT DETAILS</h6>
                        <li>
                            <div class="d-flex">
                                <i class="bi bi-house-door-fill me-3 icons_color"></i>
                                <span>12345 North Main Street, New York, NY 555555</span>
                            </div>
                        </li>
                        <li>
                            <div class="d-flex align-items-center">
                                <i class="fa-solid fa-phone me-3 icons_color rotate_x"></i>
                                <span>1.800.555.6789</span>
                            </div>
                        </li>
                        <li>
                            <div class="d-flex align-items-center">
                                <i class="fa-regular fa-envelope me-3 icons_color"></i>
                                <span>info@your-domain.com</span>
                            </div>
                        </li>
                        <li>
                            <div class="d-flex align-items-center">
                                <i class="fa-solid fa-link me-3 icons_color"></i>
                                <span>Theme-Fusion.com</span>
                            </div>
                        </li>
                    </ul>
                </div>
                <div id="courses_list" class="col-3">
                    <ul class="green_color">
                        <h6 class="text-white mb-4">COURSES</h6>
                        <li>
                            <div class="d-flex align-items-center">
                                <i class="fa-regular fa-circle-right me-3"></i>
                                <span>Pass Plus</span>
                            </div>
                        </li>
                        <li>
                            <div class="d-flex align-items-center">
                                <i class="fa-regular fa-circle-right me-3"></i>
                                <span>Intensive Course</span>
                            </div>
                        </li>
                        <li>
                            <div class="d-flex align-items-center">
                                <i class="fa-regular fa-circle-right me-3"></i>
                                <span>Automatic</span>
                            </div>
                        </li>
                        <li>
                            <div class="d-flex align-items-center">
                                <i class="fa-regular fa-circle-right me-3"></i>
                                <span>Instructor Training</span>
                            </div>
                        </li>
                    </ul>
                </div>
                <div class="col-3 d-flex flex-column align-items-center">
                    <img class="img-fluid" src="../assets/images/footer-ad-grid.png" alt="">
                    <button>BOOK NOW</button>
                </div>
            </div>
        </div>
    </div>
    <div id="bottom_footer">
        <div class="container">
            <div class="row">
                <div class="col-12 d-flex justify-content-between">
                    <span>© Copyright 2012-2020 | Avada Theme by <span class="green_color">ThemeFusion</span> | all Rights Reserved | Powered by <span class="green_color">WordPress</span></span>
                    <div class="text-white fs-6">
                        <i class="fa-brands fa-facebook-f me-4"></i>
                        <i class="fa-brands fa-twitter me-4"></i>
                        <i class="fa-brands fa-youtube me-4"></i>
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                </div>
            </div>
        </div>
    </div>
  
</template>

<style scoped>

.green_color {
    color: #7ABC64;
}

#top_footer {
    background-image: url("../assets/images/footer-background-color.jpg");
    background-size: cover;


    p {
        color: grey;
        margin-top: 20px;
        line-height: 30px;
    }

    .icons_color {
        color: rgb(202, 202, 202);
    }

    .rotate_x {
        transform: rotate(-90deg);
    }

    button {
        font-size: 14px;
        font-weight: bolder;
        background-color: #7ABC64;
        color: white;
        padding: 8px 28px;
        border: none;
        border-radius: 25px;
        cursor: pointer;
        margin-top: 25px;
        transition: background-color 0.3s ease-in-out;
    }

    ul {
        list-style-type: none;
        padding: 0;
        margin: 0;

        li {
            margin-top: 15px;
            margin-bottom: 20px;

            span {
                font-size: 14px;
                padding-right: 90px;
                line-height: 25px;
            }
        }
    }

    #courses_list {
        span {
            font-size: 18px;
        }
    }
}

#bottom_footer {
    background-color: rgb(29, 29, 29);
    font-size: 10px;
    padding: 50px;
    color: rgb(95, 95, 95);
}

</style>
