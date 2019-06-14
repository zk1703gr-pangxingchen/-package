<template>
	<view class="content">
		<view class="top">
			<!-- 搜索框  消息 -->
				<!-- <view><input type="text" class="input" placeholder="请输入"></view> -->
				<view class="i">
					<input type="text" class="input" placeholder="一键查询包裹">
					<image src="../../static/img/xx.png" mode="" class="img" ></image>					
				</view>
				<!-- 轮播图 -->
				<view class="lb">
					<uni-swiper-dot :info="info" :current="current" field="content" :mode="mode">
						<swiper class="swiper-box" @change="change" autoplay="autoplay">
							<swiper-item v-for="(item ,index) in info" :key="index">
								<view class="swiper-item">
									<image :src="item.content" mode=""></image>
								</view>
							</swiper-item>
						</swiper>
					</uni-swiper-dot>
				</view>
				<!-- 宫格 -->
				<gongge></gongge>
				<!-- 近日签收 -->
				<!-- <uni-swipe-action :options="options"> -->
					<view class='cont'>
						<view style="font-size: 40upx;font-weight: bold;margin-left: 20upx;">近日签收</view>
						<view class="qs">
							<image src="../../static/img/qs.jpg" mode=""></image>
							<view style="display: inline-block;">
								<view class="wz1">已签收</view>
								<view class="wz2">天猫|【254797】买的【...</view>
								<view class="g"><image src="../../static/gongge/g1.png" mode=""></image></view>
							</view>
							
						</view>
					</view>
				<!-- </uni-swipe-action> -->
				
				<love></love>
		</view>
		
			
		
	</view>
</template>

<script>
	import uniNavBar from "@/components/uni-nav-bar/uni-nav-bar.vue"
	import uniSwiperDot from "@/components/uni-swiper-dot/uni-swiper-dot.vue"
	// import uniSwipeAction from "@/components/uni-swipe-action/uni-swipe-action.vue"
	import gongge from "../zujian/gongge.vue"
	import love from "../zujian/love.vue"
	export default {
		components: {uniNavBar,uniSwiperDot,gongge,love},
		data() {
			return {
				 info: [
					 {content: '../../static/lunbo/lb3.jpg'},
					 {content: '../../static/lunbo/lb4.png'},
					 ],
					current: 0,
					mode: 'default',
					// options: [{
					// 		text: '取消',
					// 		style: {
					// 			backgroundColor: '#007aff'
					// 		}
					// 	}, {
					// 		text: '确认',
					// 		style: {
					// 			backgroundColor: '#dd524d'
					// 		}
					// 	}]
					}
		},
		mounted() {
			
		},
		methods:{
			change(e) {
				this.current = e.detail.current;
			}
		}
	}
</script>

<style>
	@import url("../../static/css/home.css");
	/* .content {
		margin-top: 50upx;
		text-align: center;
		height: 400upx;
	}

	.title {
		font-size: 36upx;
	} */
</style>
