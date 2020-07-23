<template>
  <div class="container">
    <div class="main">
      <div
        class="project"
        v-for="(item, index) in list"
        :key="index"
      >
        <p class="name">{{item.name}}</p>
        <div class="header">
          <p>{{item.time}}</p>
          <p>{{item.work}}</p>
        </div>
        <div class="content">
          <p
            v-for="(s, i) in item.desc"
            :key="i"
          >{{s}}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data: {
      list: [{
        name: '社内私有云 FOne HCI 超融合',
        time: '2020.3 - 2020.7',
        work: '多平台前端开发',
        desc: ['1. 参与回收站、备份、项目组架构、配额等业务需求的开发；', '2. 主导整合 storageJump、cloudJump 等系统平台的 UI 统一，体验优化；', '3. 搭建 mock server 平台并在团队中推广，提高前后端工作效率；', '4. 多次参与项目内技术分享活动，与团队共同学习成长。']
      }, {
        name: '华为云文档数据库 DDS、多模 Nosql 数据库 Geminidb 控制台',
        time: '2018.9 - 2020.3',
        work: '价格计算器及控制台管理后台前端开发',
        desc: ['1. 参与 DDS 功能需求的开发，官网价格计算器的月度版本迭代和上线；', '2. 基于 ng7 搭建了 Geminidb(多模 NoSQL 数据库)项目结构并完成了 70%业务代码的开发；', '3. 输出国际化词条转换 excel 工具(重复词检测、excel 解析和生成)，提高了团队的工作效率；', '4. 基于 Selenium 等工具编写测试代码协助持续集成与自动化测试，保证代码的可靠和安全。']
      }, {
        name: '家政加',
        time: '2018.1 - 2018.7',
        work: 'rn微应用开发',
        desc: ['1. 参与 React-Native 构建开发原生 app，封装提取公共组件、处理跨平台兼容性问题；', '2. 负责家政加 app 的阿姨管理，组织架构、优惠券促销等功能需求开发；', '3. 开发注册有礼和准点秒杀活动相关页面，并输出通用参数配置，方便运营人员修改。']
      }, {
        name: 'PC 端 e 家政管理系统',
        time: '2017.8 - 2018.1',
        work: '管理后台前端开发',
        desc: ['1. 担任 e 家政 PC 端管理系统的前端开发工作，重视组件封装与模块复用。使用 React 技术栈，利用 Echarts 渲染仪表盘/图表功能，封装 Handsontable 完成工作表、电子表格功能；', '2. 独立负责开发阿姨简历、面试流程、认证管理、快速收款等功能模块；', '3. 设计和封装表单、表格以及上传等公共组件，方便团队成员的复用提升开发效率。']
      }, {
        name: '智能大数据应用分析平台',
        time: '2017.2 - 2017.6',
        work: '前后端开发',
        desc: ['1. 负责项目部分前台界面模块、后台管理模块的排版布局、交互效果及业务功能开发；', '2. 基于 UI 图将常用场景组件化，开发菜单栏、提示弹窗、图片上传、富文本编辑器等公用组件。']
      }]
    },
    onShareAppMessage () {
      return {
        title: '陈宇的简历',
        path: '/pages/basic/main'
      }
    }
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
    .project {
      margin: 40rpx;
      @include flex(column, flex-start, flex-start);
      .name {
        @include font(40, #1296db, 40, 600);
        text-align: left;
      }
      .header {
        margin-top: 40rpx;
        @include flex(row, space-between, center);
        flex-wrap: wrap;
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
