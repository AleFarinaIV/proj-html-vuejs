<script>
import FooterItem from "./FooterItem.vue"
import { footer_lists } from "../data/footerData.js"
export default {
    components: {
        FooterItem,
    },
    data() {
        return {
            footer_lists,
        }
    }

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
                    <p>
                        Avada Driving School is the right choice for experienced drivers looking for a refresher course, 
                        or the brand new driver wanting to pass first time.
                    </p>
                </div>

                <FooterItem v-for="list, index in footer_lists"
                :key="index"
                :list="list"/>

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


#top_footer {
    background-image: url("../assets/images/footer-background-color.jpg");
    background-size: cover;


    p {
        color: grey;
        margin-top: 20px;
        line-height: 30px;
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
