<template>
	<view class="home">
		<view class="box">
			<view class="left">
					<i :class="style[img] "/>
			</view>
			<view class="right" >
				<view class="text">
						<view class="top">
							<view class="title" v-if="title" >{{title}}</view>
							<view class="money" v-if="money">￥<text>{{money}}</text></view>
						</view>
						<view class="info" v-if="info">
							{{info}}
						</view>
						<view class="time" v-if="time">
							{{time}}
						</view>
					</view>
				</view>
				<view class="into" v-if="icon" />	
		</view>
	</view>
</template>

<script>
	export default{
		props:{
				// 图标	 
			 img:{
				 type:String,
				 default:''
			 },
			 // 标题
			 title:{
				 type:String,
				 default:''
			 },
			 // 内容
			 info:{
				 type:String,
				 default:''
			 },
			 // 时间
			 time:{
				 type:String,
				 default:''
			 }, 
			 // 价钱
			 money:{
				 type:String,
				 default:''
			 },
			 // 进入图标
			 icon:{
				 type:String,
				 default:''
			 }
			
		},
		data(){
			return {
				style:{
					"floor":"floor",
					"water":"water",
					"electric":"electric"
				}
			}
		}
	}
</script>

<style scoped>
	@import url("./index.scss");
</style>
