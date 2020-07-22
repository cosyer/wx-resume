<template>
  <div class="container">
    <div class="main">
      <div class="work">
        <p class="time">2018.9-至今</p>
        <div class="header">
          <p>南京富士通南大软件技术有限公司</p>
          <p>前端开发</p>
        </div>
        <p class="content">
          1. 负责社内私有云项目需求研发、UI 改善、公共组件封装、项目性能优化、前端人员技术面试<br>
          2. 外派参与华为云 DDS(文档型数据库)和多模 Nosql 数据库 Geminidb 控制台项的开发工作
        </p>
      </div>
      <div
        class="work"
        style="margin-top: 80rpx"
      >
        <p class="time">2017.8-2018.8</p>
        <div class="header">
          <p>江苏千米网络科技股份有限公司</p>
          <p>前端开发</p>
        </div>
        <p class="content">
          1. 负责 e 家政 PC 端管理系统和家政加 APP 的前端开发工作，以及上线后功能的迭代与优化；<br>
          2. 参与 c 端小程序和公众号 H5 页面的维护和开发。
        </p>
      </div>
      <div
        class="work"
        style="margin-top: 80rpx"
      >
        <p class="time">2016.6-2017.7</p>
        <div class="header">
          <p>重庆新媒农信科技有限公司</p>
          <p>java web实习生</p>
        </div>
        <p class="content">
          1. 负责公司官网页面的重构和维护；<br>
          2. 搭建项目架构，前后台分离开发。同时编写后台接口填补页面交互逻辑；<br>
          3. 学习了开发基础知识和规范的项目流程，实现了从新人到 IT 入门的转变。
        </p>
      </div>
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
    .work {
      margin: 40rpx;
      @include flex(column, flex-start, flex-start);
      .time {
        @include font(40, #1296db, 40, 600);
        text-align: left;
      }
      .header {
        margin-top: 40rpx;
        @include flex(row, space-between, center);
        p {
          display: inline-block;
          @include font(32, #000, 40, 500);
        }
      }
      .content {
        margin-top: 40rpx;
        text-align: left;
        @include font(28, #444, 36, 400);
      }
    }
  }
}
</style>
