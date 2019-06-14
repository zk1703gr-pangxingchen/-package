<template>
	<view class="content">
		<view>
			<view class="v1" style="background: #FFFFFF;">
				<image src="../../static/post/1.png" mode="aspectFit"></image>
				<view class="v2">附近暂无驿站</view>
			</view>
			<view class="v3">
				<view class="text">
					您可以选择速递之家-上门取件服务
				</view>
				<view class="a1">
					<image src="../../static/post/2.png" mode="aspectFit"></image>
					<view class="a2">
						时效保障
					</view>
					<view class="a3">
						2小时内上门取件,免收上门费
					</view>
				</view>
				<view class="b1">
					<image src="../../static/post/3.png" mode="aspectFit"></image>
					<view class="a2">
						安全保障
					</view>
					<view class="a3">
						货丢货损,速递之家全程跟踪赔付
					</view>
				</view>
				<view class="b1">
					<image src="../../static/post/4.png" mode="aspectFit"></image>
					<view class="a2">
						安全保障
					</view>
					<view class="a3">
						货丢货损,速递之家全程跟踪赔付
					</view>
				</view>
				<view>
					<button class="button" @click="fn">马上寄件</button>
				</view>
			</view>

		</view>

	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		mounted() {

		},
		methods: {
			fn() {
				uni.switchTab({
					url: '/pages/index/mailing'
				});
			}
		}
	}
</script>

<style>
	page {
		background: #F4F4F4;
	}

	.content {
		margin-top: 65upx;
	}

	.v1 {
		height: 400upx;
	}

	.v1 image {
		height: 250upx;
		margin-left: 40upx;
	}

	.v2 {
		font-size: 25upx;
		text-align: center;
		margin: 30upx 0;
	}

	.v3 {
		height: 740upx;
		margin-top: 40upx;
		background: #FFFFFF;
		padding: 50upx 0;
	}

	.text {
		background: #007AFF;
		width: 80%;
		height: 50upx;
		font-size: 25upx;
		text-align: center;
		line-height: 50upx;
		margin-left: 10%;
		color: #FFFFFF;
		border-radius: 40upx;
	}

	.a1 {
		margin-top: 40upx;
	}

	.a1 image {
		height: 80upx;
		width: 80upx;
		display: inline-block;
		margin-top: 50upx;
		margin-left: 15%;
	}

	.a2 {
		display: inline-block;
		font-size: 30upx;
		font-weight: bold;
		vertical-align: top;
		line-height: 120upx;
		margin-left: 40upx;
	}

	.a3 {
		display: inline-block;
		font-size: 25upx;
		margin-left: -120upx;
	}

	.b1 image {
		height: 80upx;
		width: 80upx;
		display: inline-block;
		margin-top: 50upx;
		margin-left: 15%;
	}

	.button {
		margin-top: 80upx;
		width: 95%;
		border-radius: 50upx;
		background: #007AFF;
		color: #FFFFFF;
		height: 100upx;
		font-size: 30upx;
		line-height: 100upx;
	}
</style>
