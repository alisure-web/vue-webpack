<style>
    .my-button{
        text-align: center;
        display: inline-block;
        user-select: none;
        cursor: pointer;
    }

    .my-button.theme-1{
        background-color: #7f7f7f;
    }
    .my-button.theme-1:hover{
        background-color: cadetblue;
    }
    .my-button.theme-1:active{
        background-color: chartreuse;
    }

    .my-button.theme-2{
        background-color: #ead49d;
    }
    .my-button.theme-2:hover{
        background-color: #eacc71;
    }
    .my-button.theme-2:active{
        background-color: #eac43e;
    }
</style>

<template>
    <div class="my-button" :class="theme"
         :style="{'width':width, 'height':height, 'line-height':height,
         'border-radius':radius, 'font-size': fontSize}"
         @click.prevent="clickButton($event)"
    >
        {{text}}
    </div>
</template>

<script>
    export default {
        name: "myButton",
        data() {
            return {

            }
        },
        props: {
            text: {
                type: String,
                default: "按钮",
                required: true
            },
            width: {
                type: String,
                default: "32px"
            },
            height: {
                type: String,
                default: "64px"
            },
            radius: {
                type: String,
                default: "5px"
            },
            fontSize: {
                type: String,
                default: "14px"
            },
            theme: {
                type: String,
                default: "theme-1"
            }
        },
        methods: {
            clickButton: function (event) {
                this.$emit("clickButton");
            }
        }
    }
</script>
