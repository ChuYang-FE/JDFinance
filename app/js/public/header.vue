<template>
  <div :class="$style.header">
    <span :class="$style.left">
      <em>注册</em>&nbsp;|&nbsp;<em>登录</em>
    </span>
    <btn :class="$style.btnDownload">APP下载</btn> <!--btn.vue里定义了slot插槽，直接写入文本-->
  </div>
</template>

<script>
import btn from "../core/btn"
export default {
  components:{
    btn,
  },
}
</script>

<style lang="scss" module> //用module把样式局域化，防止全局干扰。
  .header{
    color: #666;
    height: 100px;
    line-height: 100px;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    font-size: 32px;
    background: #fff url(//storage.360buyimg.com/base/images/jdjr-logo/logo-jr-r.png?20181203) center center no-repeat;
    background-size: auto 50%;
    z-index: 100;
    .left{
      font-size: 28px;
      height: 30px;
      line-height: 30px;
      margin: 17px 0 0 18px;
    }
    .btnDownload{
      float: right;
      font-size: 24px;
      border-width: 0;
      height: 56px;
      line-height: 56px;
      min-width: 120px;
      padding: 0;
      border-radius: 4px;
      margin: 28px 24px 0 0;
    }

  }
</style>