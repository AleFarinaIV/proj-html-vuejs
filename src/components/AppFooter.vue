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
                        <h6 class="text-white">CONTACT DETAILS</h6>
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
                <div class="col-3"></div>
                <div class="col-3"></div>
            </div>
        </div>
    </div>
    <div id="bottom_footer">

    </div>
  
</template>

<style scoped>

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

    ul {
        list-style-type: none;
        padding: 0;
        margin: 0;

        li {
            margin-top: 15px;
            margin-bottom: 20px;

            span {
                font-size: 14px;
                padding-right: 80px;
                line-height: 25px;
            }
        }
    }
}

</style>
