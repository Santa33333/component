<template>
	<view class="content">
		<view class="comment"></view>
		<view class="center">
			<image src="../../static/image.jpg"></image>
			<view class="title">
				<text>Diana Vahed</text>
			</view>
			<text class="photograph">Hey Everyone, this is Dianna Vahed from Lebanon. I’m interaction designer with more than 8 years of experience working as a Product designer in SoftCo Ltd。Hey Everyone, this is Dianna Vahed from Lebanon. I’m interaction designer with more than 8 years of experience working as a Product designer in SoftCo Ltd</text>
			<view class="botton">
				<view class="follow" @click="handleClick">
					<text>Follow</text>
				</view>
				<view class="fly" @click="sendClick">
					<view class="circle">
						<image src="../../static/Vector.png"></image>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {
			handleClick(){
				uni.navigateTo({
					url:'/pages/about/about'
				});
			},
			sendClick(){
				console.log('成功点击too');
			}
		}
	}
</script>

<style>
	.content{
		width: 706rpx;
		height: 539.94rpx;
		margin: 100px auto;
		position: relative;
	}
	
	.comment{
		width: 353px;
		height: 226.894px;
		flex-shrink: 0;
		border-radius: 30px;
		background: #FFF;
		box-shadow: 0px 10px 20px 0px rgba(0, 95, 183, 0.30);
		position: absolute;
		bottom: 0;
	}
	
	.center{
		display: flex;
		width: 319px;
		flex-direction: column;
		align-items: center;
		gap: 15px;
		position: absolute;
		margin-left: 18px;
	}
	
	.center image{
		width: 92.59px;
		height: 86.094px;
		border-radius: 50%;
	}
	
	.center .title{
		width: 120px;
		height: 30px;
		color: #000;
		font-family: Roboto;
		font-size: 18px;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
		text-align: center;
	}
	
	.center .photograph{
		display: -webkit-box;
		-webkit-box-orient: vertical;
		-webkit-line-clamp: 3;
		align-self: stretch;
		overflow: hidden;
		color: #000;
		text-align: center;
		text-overflow: ellipsis;
		font-family: Roboto;
		font-size: 12px;
		font-style: normal;
		font-weight: 400;
		line-height: normal;
		margin-top: -10px;
	}
	
	.center .botton{
		display: flex;
		width: 302.117px;
		justify-content: center;
		align-items: center;
		gap: 20px;
	}
	
	.center .botton .follow{
		display: flex;
		padding: 14px 87px;
		justify-content: center;
		align-items: center;
		gap: 10px;
		flex-shrink: 0;
		border-radius: 12px;
		background: #046BA5;
	}
	
	.center .botton .follow text{
		color: #FFF;
		text-align: center;
		font-family: Roboto;
		font-size: 18px;
		font-style: normal;
		font-weight: 800;
		line-height: normal;
	}
	
	.center .botton .fly{
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		gap: 10px;
	}
	
	.center .botton .fly .circle{
		width: 51.117px;
		height: 48.428px;
		border-radius: 12px;
		background: rgba(4, 107, 165, 0.20);
	}
	
	.center .botton .fly image{
		width: 18px;
		height: 17px;
		position: relative;
		left: 16.229px;
		top: 15.394px;
		fill: #046BA5;
	}
</style>
