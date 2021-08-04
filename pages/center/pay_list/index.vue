<style scoped lang='scss'>
	@import 'index.scss';
</style>
<template>
	<view class='pay-list'>
		<view class="up">
				<scroll-view scroll-y>
					<view class="top-box page-section swiper">
						<view class="page-section-spacing">
								<swiper class="swiper" >
										<swiper-item><image src="/static/img/banner.png" mode=""></swiper-item>
								</swiper>
						</view>
					</view>
					<view class="center-box">
						<view class="top">
							<view class="my-payment">我的缴费</view>
							<view class="record">缴费记录</view>
						</view>
						<view class="center">
							<template v-for="(item,id) in paymentList" >
								<view class="center-block">
										<community 
											:key="id"
											:img="item.img"
											:title="item.title"
											:info = "item.info"
											:icon = "item.icon"
											:money = "item.money"
											:time = "item.time"
										></community>
								</view>
							
								<view class="border" />
							</template>
						</view>
					</view>	

				</scroll-view>
		</view>
		<view class="bottom">
			<button type="default" class="btn">
					+ 新增小区
			</button>
		</view>
	</view>
</template>
<script>
import community from '@/components/community/index.vue'
export default {
	data(){
		return{
			background: ['color1', 'color2', 'color3'],
			indicatorDots: true,
			autoplay: true,
			interval: 2000,
			duration: 500,
			bannerList: [{
					image: '/static/img/banner1@2x%20(1).png',
					title: '昨夜星辰昨夜风，画楼西畔桂堂东'
				},
				{
					image: 'https://cdn.uviewui.com/uview/swiper/2.jpg',
					title: '身无彩凤双飞翼，心有灵犀一点通'
				},
				{
					image: 'https://cdn.uviewui.com/uview/swiper/3.jpg',
					title: '谁念西风独自凉，萧萧黄叶闭疏窗，沉思往事立残阳'
				}
			],
			paymentList:[{	
				title:"海滨华庭小区(住宅区)",
				img:"floor",
				info:"11栋1602户",
				icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				},{	
					title:"中骏·雍景台(商品房)",
					img:"floor",
					info:"11栋1602户",
					icon:"icon",
				}
			],
		
		}
	},
	components:{
		community
	},
	computed:{
	},
	methods: {
	},
	// onLoad(options) {
	// 	console.log('onLoad监听页面加载');
	// },
	// onReady() {
	// 	console.log('onReady监听页面初次渲染完成');
	// },
	// onShow() {
	// 	console.log('onShow监听页面显示');
	// },
	// onHide() {
	// 	console.log('onHide监听页面隐藏');
	// },
	// onUnload() {
	// 	console.log('onUnload监听页面卸载');
	// },
	
}
</script>