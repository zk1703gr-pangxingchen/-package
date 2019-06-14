<template>
	<view>
		<view style="background: #F4F4F4;">
			<view style="background: #FFFFFF;">
				<cmd-cell-item title="新消息通知" arrow hover-class="cel-item-hover"></cmd-cell-item>
				<cmd-cell-item title="取件提醒"  arrow hover-class="cel-item-hover"></cmd-cell-item>
				<cmd-cell-item title="驿站取件通知消息设置"  arrow hover-class="cel-item-hover"></cmd-cell-item>
			</view>
			
			<view style="margin-top: 50upx;background: #FFFFFF;">
				<cmd-cell-item title="关于裹裹" arrow hover-class="cel-item-hover"></cmd-cell-item>
				<cmd-cell-item title="使用条款" arrow hover-class="cel-item-hover"></cmd-cell-item>
				<cmd-cell-item title="检查更新" addon="目前是最新版本" arrow hover-class="cel-item-hover"></cmd-cell-item>
			</view>
			<view style="margin-top: 50upx;background: #FFFFFF;">
				<cmd-cell-item title="隐私" arrow hover-class="cel-item-hover"></cmd-cell-item>
			</view>
			
			<button type="default" style="margin-top: 50upx;background: #FFFFFF;">退出登录</button>
		</view>
		
	</view>
</template>

<script>
	import cmdCellItem from '@/components/cmd-cell-item/cmd-cell-item.vue'
	export default {
		components: {cmdCellItem},
		data() {
			return {

			}
		},
		mounted() {
			
		},
		methods:{
			
		}
	}
</script>

<style>
	.content {
		margin-top: 50upx;
		text-align: center;
		height: 400upx;
	}

	.title {
		font-size: 36upx;
	}
</style>
