<script>
import { footer_lists } from "../data/footerData.js"

export default {
    data() {
        return {
            footer_lists,
        }
    },
    props: {
        list: Object,
    }
}
</script>

<template>

    <div class="col-3">
        <ul :class="list.ul_class">
            <h6 class="text-white mb-4">{{list.title}}</h6>
            <li v-for="el in list.list">
                <div class="d-flex" :class="{'align-items-center' : el.isAlignStart == false}">
                    <i :class="el.icon_class"></i>
                    <span :class="el.span_class">{{el.text}}</span>
                </div>
            </li>
        </ul>
    </div>

</template>

<style scoped lang="scss">

    .fs-18 {
        font-size: 18px;
    }

    .rotate_x {
        transform: rotate(-90deg);
    }

    .icons_color {
        color: rgb(202, 202, 202);
    }

    .green_color {
        color: #7ABC64;
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
                cursor: pointer;
            }
        }
    }

</style>