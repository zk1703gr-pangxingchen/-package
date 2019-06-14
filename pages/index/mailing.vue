<template>
	<view class="content">
		<view class="s">
			<image src="../../static/img/shijian.png" mode="aspectFit"></image>
			<view>寄件记录</view>
		</view>
		<!-- 选项卡 -->
		<view class="s1">
			<wuc-tab :tab-list="tabList" :tabCur.sync="TabCur" @change="tabChange"></wuc-tab>
			<view class="a">
				<view v-show="TabCur === 0">
					<guoguo></guoguo>
				</view>
				<view v-show="TabCur === 1">
					2
				</view>
				<view v-show="TabCur === 2">
					3
				</view>
			</view>
		</view>

	</view>
</template>

<script>
	import WucTab from '@/components/wuc-tab/wuc-tab.vue';
	import guoguo from '../zujian/guoguo.vue'
	export default {
		components: {
			WucTab,guoguo
		},
		data() {
			return {
				TabCur: 0,
				tabList: [{
					name: '裹裹寄件'
				}, {
					name: '驿站寄件'
				}, {
					name: '公益寄件'
				}],
			}
		},
		mounted() {

		},
		methods: {
			tabChange(index) {
				if (this.current !== index) {
					this.current = index;
				}
			}
			// tabChange(index) {
			// 	this.TabCur = index;
			// }
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

	.title {
		font-size: 36upx;
	}

	.s view {
		height: 50upx;
		width: 200upx;
		font-size: 30upx;
		text-align: center;
		border-radius: 50upx;
		background: #C5CAD5;
		color: #007AFF;
		line-height: 50upx;
		float: right;
	}

	.s image {
		height: 50upx;
		width: 50upx;
		float: right;
		margin: 0 20upx;
	}
</style>
