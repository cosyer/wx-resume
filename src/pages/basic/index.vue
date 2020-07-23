<template>
  <div class="container">
    <div class="main">
      <img src="/static/images/avatar.png" />
      <p class="name">陈宇</p>
      <p></p>
    </div>
    <div class="base">
      <div class="box">
        <p>年龄: {{age}}</p>
        <p>学历: 本科</p>
        <p>所在地: 江苏南京</p>
        <p>工作经验: {{workYear}}年</p>
        <p>籍贯: 江苏扬州</p>
        <p>求职意向: 前端开发</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data: {
      age: 0,
      workYear: 0
    },
    created () {
      this.initAge()
      this.initWorkYear()
    },
    methods: {
      initAge () { // 计算年龄
        let date = new Date()
        let year = date.getFullYear()
        let month = date.getMonth() + 1
        let day = date.getDate()
        if (month > 6) {
          this.age = year - 1994
        } else {
          if (day > 4) {
            this.age = year - 1994
          } else {
            this.age = year - 1995
          }
        }
      },
      initWorkYear () { // 粗略计算工作年限
        let now = (new Date()).getTime()
        let workDay = (new Date('2017/6/30')).getTime()
        let years = (now - workDay) / (1000 * 60 * 60 * 24 * 365)
        this.workYear = Number(years).toFixed(1)
      }
    },
    onShareAppMessage () {
      return {
        title: '陈宇的简历',
        path: '/pages/basic/main'
      }
    }
  }
</script>

<style lang="scss" scoped>
@import "../../styles/comm";
.container {
  padding-top: 40rpx;
  width: 750rpx;
  height: 100%;
  @include flex(column, flex-start, center);
  .main {
    @include w_h(670, 500);
    @include flex($j: center, $a: center);
    border-radius: 8rpx;
    box-shadow: 0 10rpx 20rpx #1296db;
    img {
      @include w_h(200, 200);
      border-radius: 100rpx;
    }
    .name {
      margin-top: 40rpx;
      text-align: center;
      @include font(40, #000, 40, 600);
    }
  }
  .base {
    margin-top: 80rpx;
    width: 670rpx;
    border-radius: 8rpx;
    box-shadow: 0 10rpx 20rpx #1296db;
    .box {
      margin-top: 20rpx;
      margin-bottom: 20rpx;
      p {
        text-align: center;
        @include font(32, #000, 50, 400);
      }
    }
  }
}
</style>
