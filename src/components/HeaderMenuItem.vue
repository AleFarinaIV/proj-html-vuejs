<script>
import { menu } from "../data/headerMenuData.js";
export default {
    data() {
        return {
            menu
        }
    },
    props: {
        label: {
            type: String,
        },
        active: {
            type: Boolean,
        },
        new: {
            type: Boolean,
        }
    }
}

</script>

<template>

    <li class="d-flex align-items-center">
        <a href="#" :class="{'active' : active}" >{{ label }}</a>
        <span v-if="new" class="label ms-2">NEW</span>
    </li>

</template>

<style scoped>

    li {
        margin-right: 55px;
        font-size: 14px;
        font-weight: 700;

        a {
            color: #ffffff;
            text-decoration: none;

        }
        
        .active {
            color: #7ABC64;
            border-bottom: 2px solid #7ABC64;
        }

        .label {
            font-size: 9px;
            background-color: #7ABC64;
            padding: 2px 5px;
            border-radius: 5px;
        }
    }

</style>