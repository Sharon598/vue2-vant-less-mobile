<template>
  <div class="home">
    <van-button type="primary"> 你好,这里是主页</van-button>
    <van-collapse v-model="activeNames">
      <van-collapse-item
        title="步骤1"
        name="1"
      >首先，你需要新建 style 公共样式文件，并重置所有样式</van-collapse-item>
      <van-collapse-item
        title="步骤2"
        name="2"
      >在 main.js 中引入公共样式文件</van-collapse-item>
      <van-collapse-item
        title="步骤3"
        name="3"
      >全局样式生效</van-collapse-item>
    </van-collapse>
    <van-steps direction="vertical" :active="0">
      <van-step>
        <h3>运行： npm run serve</h3>
      </van-step>
      <van-step>
        <h3>打包： npm run build</h3>
      </van-step>
      <van-step>
        <h3>webpack配置文件：</h3>
        <p>根目录新建： vue.config.js</p>
      </van-step>
    </van-steps>
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
