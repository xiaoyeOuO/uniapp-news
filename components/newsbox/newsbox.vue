<template>
	<view class="newsbox">
		<view class="pic">
			<image src="@/static/images/0.jpg" mode="aspectFill"></image>
		</view>
		<view class="text">
			<view class="title">
				<text>新闻的默认标题新闻的默认标题新闻的默认标题新闻的默认标题新闻的默认标题</text>
			</view>
			<view class="info">
				<text>作者</text>
				<text>浏览量</text>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		name:"newsbox",
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
	.newsbox{
		display: flex;
		.pic{
			width: 230rpx;
			height: 160rpx;
			image{
				width: 100%;
				height: 100%;
			}
		}
		.text{
			flex: 1;
			padding-left: 20rpx;
			display: flex;
			justify-content: space-between;
			flex-direction: column;
			.title{
				font-size: 36rpx;
				color: #333;
				text-overflow: -o-ellipsis-lastline;
				overflow: hidden;
				display: -webkit-box;
				-webkit-line-clamp: 2;
				line-clamp: 2;
				-webkit-box-orient: vertical;
			}
			.info {
				font-size: 26rpx;
				color: #999;
				text {
					padding-right: 30rpx;
				}
			}
		}
	}
</style>