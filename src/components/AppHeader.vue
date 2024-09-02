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
        <div class="container">
            <div class="d-flex justify-content-between">
                <span>We have a 95% Successful Pass Rate!</span>
                <span>
                    <i class="bi bi-telephone-fill rotate_x me-1"></i> Give us a call to book your tuition! 1-800-555-555
                </span>
            </div>
        </div>
    </div>
    <div class="bottom_header">
        <div class="container">
            <div class="row justify-content-between align-items-center">
                <div class="col-4">
                    <img src="../assets/images/avada-drivers-logo-2x-300x58.png" alt="">
                </div>
                <div class="col-8">
                    <div class="row align-items-center">
                        <div class="col-12 d-flex justify-content-between">
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
    </div>

</template>

<style scoped>
    .top_header {
        padding: 10px;
        background-color: #494C4E;
        font-size: 14px;

        .container {
            color: rgb(160, 160, 160);

            .rotate_x {
                transform: rotate(-90deg);
            }

        }
    }

    .bottom_header {
        padding: 20px;
        background-color: rgba(0, 0, 0, 0.301);

        .container {

            button {
                font-size: 16px;
                font-weight: 700;
                background-color: #7ABC64;
                color: #ffffff;
                padding: 7px 24px;
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
</style>
