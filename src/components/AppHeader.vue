<script>
import HeaderMenuItem from "./HeaderMenuItem.vue"
import { menu } from "../data/headerMenuData.js"
export default {
    components: {
        HeaderMenuItem,
    },
    data() {
        return {
            menu,
        }
    }
}

</script>

<template>
    <div class="top_header">
        <div class="my_container">
            <div class="d-flex justify-content-between">
                <span>We have a 95% Successful Pass Rate!</span>
                <span>
                    <i class="bi bi-telephone-fill"></i>
                    Give us a call to book your tuition! 1-800-555-555
                </span>
            </div>
        </div>
    </div>
    <div class="bottom_header">
        <div class="my_container">
            <div class="d-flex justify-content-between align-items-center">
                <div class="col-4 size">
                    <img src="../assets/images/avada-drivers-logo-2x-200x39.png" alt="">
                </div>
                <div class="col-8">
                    <div class="d-flex justify-content-end align-items-center">
                        <ul class="list-unstyled d-flex ms-3 text-white m-0">
                            <HeaderMenuItem 
                            v-for="section, index in menu"
                            :key="index" 
                            :label="section.label"
                            :active="section.active"
                            :new="section.new"/>
                        </ul>
                        <button>
                            BOOK NOW
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<style scoped>
    .top_header {
        padding: 10px;
        background-color: #494C4E;
        font-size: 14px;

        .my_container {
            width: 1200px;
            margin: 0 auto;
            color: rgb(160, 160, 160);
        }
    }

    .bottom_header {
        padding: 20px;
        background-color: rgba(0, 0, 0, 0.301);

        .my_container {
            width: 1200px;
            margin: 0 auto;

            .size {
                width: 300px;
                height: 50px;
    
                img {
                    width: 100%;
                    height: 100%;
                }
            }

            button {
                font-size: 14px;
                font-weight: 700;
                background-color: #7ABC64;
                color: #ffffff;
                padding: 7px 20px;
                border: none;
                border-radius: 25px;
                cursor: pointer;
                transition: background-color 0.3s ease;
            }
        }

        
    }
</style>
