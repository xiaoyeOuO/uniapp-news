<template>
	<view class="home">
		<view class="scrollNav">
			<scroll-view scroll-x class="navScroll">
				<view class='scroll-item'>国内</view>
				<view class='scroll-item'>国内</view>
				<view class='scroll-item'>国内</view>
				<view class='scroll-item'>国内</view>
				<view class='scroll-item'>国内</view>
				<view class='scroll-item'>国内</view>
				<view class='scroll-item'>国内</view>
			</scroll-view>
		</view>
		<view class="content">
			<view class="row" v-for="item in 10">
				<newsbox></newsbox>
			</view>
		</view>
	</view>
</template>

<script>
	export default {

	}
</script>

<style lang='scss' scoped>
	.navScroll {
		height: 100rpx;
		background: #f7f8fa;
		white-space: nowrap;

		.scroll-item {
			font-size: 40rpx;
			display: inline-block;
			line-height: 100rpx;
			padding: 0 30rpx;
			color: #333;
		}

		// 除去小程序兼容差异,在小程序中没有横向滚动条
		/deep/ ::-webkit-scrollbar {
			width: 4px !important;
			height: 1px !important;
			overflow: auto !important;
			background: transparent !important;
			-webkit-appearance: auto !important;
			display: block;
		}
	}
	.content{
		padding: 30rpx;
		.row{
			border-bottom: 1px dotted #efefef;
			
		}
	}
</style>
