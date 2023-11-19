<template>
  <view>
    <text>{{ message }}</text>
    <button @click="changeMessage">Change Message</button>
  </view>
</template>
 
<script>
export default {
  data() {
    return {
      message: 'Hello, World!'
    }
  },
  methods: {
    changeMessage() {
      this.message = 'New Message'
    }
  }
}
</script>
 
<style scoped>
/* 样式代码 */
</style>