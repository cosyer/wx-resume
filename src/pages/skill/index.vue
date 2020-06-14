<template>
  <div class="container">
    <div class="main">
      <ul>
        <li>熟悉HTML5和CSS3，了解W3C标准和web语义化，熟悉原生javascript或typescript开发，了解其基本语言特性，熟悉ES6新增特性</li>
        <li>熟练使用jQuery，vue，react框架，使用过vue-cli，vuex，vue-route以及react全家桶进行开发</li>
        <li>熟悉微信小程序开发，使用过原生小程序以及mpvue，wepy等框架，进行过第三方小程序开发</li>
        <li>了解响应式页面，熟悉使用bootstrap，使用过elementUI，ant design，weui等UI库</li>
        <li>了解http协议及浏览器原理，掌握前端问题的定位方法，了解基本的前端体验提升及性能优化</li>
        <li>熟练掌握git进行协同开发</li>
        <li>使用过服务端开发语言java，使用过springboot，了解mysql数据库，能写基本的sql语句</li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    data: {},
    onShareAppMessage () {}
  }
</script>

<style scoped lang="scss">
  @import "../../styles/comm";
  .container {
    padding: 40rpx 0;
    width: 750rpx;
    @include flex(column, flex-start, center);
    .main {
      width: 670rpx;
      border-radius: 8rpx;
      box-shadow: 0 10rpx 20rpx #1296db;
      ul {
        margin: 20rpx;
        li {
          @include font(28, #444, 40, 400);
          text-align: left;
          margin: 50rpx 20rpx;
        }
      }
    }
  }
</style>
