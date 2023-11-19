<template>
	<view>
		<view>{{messages[clickCount]}}</view>
		<button @click="handleClick">click me</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				clickCount: 0,
				messages: ["消息1", "消息2", "消息3", "消息4"]
			};
		},
		methods: {
			handleClick() {
				if (this.clickCount < this.messages.length - 1) {
				        this.clickCount++;
				}
			}
		}
	}
</script>

<style scoped>
	/* 样式代码 */
</style>
