<template>
  <div class="container">
    <div class="main">
      <ul>
        <li>1. 熟悉HTML5和CSS3，了解W3C标准和web语义化，具备扎实的 javascript 基础</li>
        <li>2. 熟悉 ES6 新特性，了解 TypeScript 以及运用 Node.js（Express、Koa2）搭建后台服务</li>
        <li>3. 熟悉使用jQuery，vue，react，angular框架，使用过vue-cli，vuex，vue-router以及react全家桶进行开发</li>
        <li>4. 了解响应式页面，熟悉使用ant design，elementUI，iview等UI库</li>
        <li>5. 了解常用的 Linux 命令，熟悉项目常规开发流程、开发调试技巧、发布部署步骤</li>
        <li>6. 了解http协议及浏览器原理，掌握前端问题的定位方法，了解基本的前端体验提升及性能优化</li>
        <li>7. 熟悉使用 Git 进行版本控制和代码托管、Markdown 进行文档编写</li>
        <li>8. 了解 Java 语言以及 MySQL、MongoDB 等数据库，运用 spring-boot 框架开发后台接口，能写基本的sql语句</li>
        <li>9. 能够科学上网，独立解决问题。遵守开发规范，有良好的文档阅读能力和代码编写习惯</li>
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
