<template>
	<view class="center">
		<view class="component">
			<MyComponent></MyComponent>
		</view>
		<view class="footer">
			<MyFooter></MyFooter>
		</view>
		<view class="back">
			<BackHome></BackHome>
		</view>
	</view>
</template>

<script>
	import MyComponent from "@/components/MyComponent/MyComponent.vue";
	import MyFooter from "@/components/MyFooter/MyFooter.vue";
	import BackHome from "@/components/BackHome/BackHome.vue";
	export default {
		components:{
			MyComponent,
			MyFooter,
			BackHome
		}
	}
</script>

<style>
	.component{
		margin-bottom: 100px;
	}
	.footer{
		margin-top: 100px;
	}
	.back{
		margin-top: 100px;
		
	}
</style>
