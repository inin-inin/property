<style scoped lang='scss'>
	@import 'index.scss';
</style>
<template>
	<div class=''>
		<div class='box' @click="to">
			asdasd
		</div>
	</div>
</template>
<script>
export default {
	components:{},
	data(){
		return {
		}
	},
	computed:{
	},
	methods: {
		to(){
			uni.navigateTo({
				url:'/pages/main/service/index'
			})
		}
	},
	onLoad(options) {
		console.log('onLoad监听页面加载');
	},
	onReady() {
		console.log('onReady监听页面初次渲染完成');
	},
	onShow() {
		console.log('onShow监听页面显示');
	},
	onHide() {
		console.log('onHide监听页面隐藏');
	},
	onUnload() {
		console.log('onUnload监听页面卸载');
	},
	
}
</script>