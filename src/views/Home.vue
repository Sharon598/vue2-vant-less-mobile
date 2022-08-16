<template>
  <div class="home">
    你好,这里是主页
    <p>首先，你需要新建 style 公共样式文件，并重置所有样式</p>
    <p>在 main.js 中引入公共样式文件</p>
    <p>全局样式生效</p>
    <Button type="primary">11111</Button>
    <van-button type="primary">主要按钮</van-button>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      activeNames: ['1']
    }
  }
}
</script>

<style lang="less" scoped>
.home {
  font-size: 12px;
}
</style>
