<template>
	<div id="content">
        <a href="./index.html">index</a>
		<my-button theme="theme-1" text="home" height="32px"
				   width="64px" font-size="14px" @clickButton="myButtonClick"></my-button>
	</div>
</template>

<script>
    import myButton from '../../components/common/button.vue'

    export default {
        name: 'app',
        components: {
            myButton
        },
        methods: {
            myButtonClick: function () {
                alert("点击按钮");
                location.href = "./index.html"
            }
        }
    }
</script>

<style>
	#content {
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}
</style>

