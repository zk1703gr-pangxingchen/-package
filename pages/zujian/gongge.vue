<template>
	<view>
		<view style="font-size: 9px;">
			<uni-grid  :options="[
				{image:'../../static/gongge/kuaidi.png',text:'寄快递'},
				{image:'../../static/gongge/gj.png',text:'领果酱'},
				{image:'../../static/gongge/xin.png',text:'我的亲友'},
				{image:'../../static/gongge/shu.png',text:'精灵书屋'},
				{image:'../../static/gongge/xiniu.png',text:'蓝犀牛'},
				{image:'../../static/gongge/huishou.png',text:'手机回收'},
				{image:'../../static/gongge/baoguo.png',text:'包裹大作战'},
				{image:'../../static/gongge/wanju2.png',text:'玩具租赁'},
				{image:'../../static/gongge/zu.png',text:'数码租赁'},
				{image:'../../static/gongge/nv.png',text:'女装租赁'},
				]" 
				show-border="false" column-num="5">
			</uni-grid>
		</view>
		
	</view>
</template>

<script>
	import uniGrid from "@/components/uni-grid/uni-grid.vue"
	export default {
		 components: {uniGrid},
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
	
</style>
