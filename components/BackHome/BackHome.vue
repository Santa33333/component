<template>
	<view>
		<button @click="goHome">backhome</button>
	</view>
</template>

<script>
	export default{
		methods:{
			goHome(){
				uni.navigateTo({
					url:'/pages/index/index'
				});
			}
		}
	}
</script>

<style>
</style>
