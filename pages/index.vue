<!--
* 一个template标签用于定义组件的模板部分, 模板是组件的HTML结构, 描述了组件的布局和内容
* 一个style标签用于定义组件的样式部分, 包含了组件的CSS样式
* 一个script标签用于定义组件的逻辑部分, 包含了组件的数据、方法、生命周期钩子等
* 一个div标签是一个块级元素, 用于定义定一个分区或节, 用于将内容分组
-->

<!--全局样式-->
<style scoped>
  .section-yellow {
    background-color: #fff8f4;
  }
  .section-gray {
    background-color: #fafafa;
  }
</style>

<!--当前页面整体布局-->
<template>
  <!--页眉导航栏-->
  <Nav class="section-yellow"></Nav>

  <!--第一块-->
  <div class="w-full section-bg section-yellow pt-20">
    <div class="w-full max-w-screen-xl m-auto px-4 lg:px-10 pb-10 lg:pb-20 flex items-center flex-wrap">
      <div class="w-full lg:w-1/2">
        <h1 class="text-center lg:text-left text-3xl lg:text-5xl pt-10 lg:pt-20">每日朋友圈</h1>
        <div class="text-center lg:text-left mt-8 text-gray-600">每日名言、节日祝福、朋友圈文案配图，打造个性化朋友圈。</div>
        <div class="mt-10 flex flex-col lg:flex-row justify-center lg:justify-start">
          <a class="bg-cus-active text-white px-4 py-3 rounded flex items-center justify-center w-48 m-auto lg:ml-0 lg:mr-0" href="/editor" target="_self">
            <span class="ml-1">
                免费使用
            </span>
          </a>
        </div>
      </div>
      <div class="w-full lg:w-1/2 lg:px-5">
        <img src="/svg/main.svg" class="max-w-screen-md m-auto">
      </div>
    </div>
  </div>

  <!--第二块-->
  <div class="w-full max-w-screen-xl m-auto px-4 lg:px-10 py-20 flex items-center flex-wrap flex-col-reverse lg:flex-row">
      <div class="w-full lg:w-1/2 lg:pr-20">
          <img src="/svg/block-1.svg" class="rounded shadow-2xl w-full max-w-sm m-auto">
      </div>
      <div class="w-full lg:w-1/2 lg:pl-10 text-center lg:text-left mb-6 lg:mb-0">
          <h2 class="text-4xl">轻松编辑，简单操作</h2>
          <div class="mt-8 text-gray-600">拒绝千篇一律，让你的朋友圈与众不同...</div>
      </div>
  </div>

  <!--第三块-->
  <div class="w-full section-bg section-gray">
      <div class="w-full max-w-screen-xl m-auto px-4 lg:px-10 py-20 flex items-center bg-yellow w-full flex-wrap text-center lg:text-left mb-6 lg:mb-0">
          <div class="w-full lg:w-1/2">
              <h2 class="text-4xl">每一天都是新鲜的，美好每时每刻</h2>
              <div class="mt-8 text-gray-600">每天新内容，有爱、有温度...</div>
          </div>
          <div class="w-full lg:w-1/2">
              <img src="/svg/block-2.svg" class="max-w-sm m-auto">
          </div>
      </div>
  </div>

  <!--第四块-->
  <div class="w-full section-bg section-yellow">
      <div class="w-full max-w-screen-xl m-auto px-4 lg:px-10 py-20 flex items-center bg-yellow w-full flex-wrap text-center mb-6 lg:mb-0">
          <div class="w-full">
              <h2 class="text-3xl">如何使用</h2>
          </div>
          <div class="w-full flex flex-wrap mt-10 justify-center">
              <div class="w-full lg:w-4/12 flex items-center">
                  <div class="w-16 h-16 border-2 border-cus-active rounded-full flex items-center justify-center font-bold number">1</div>
                  <div class="ml-6 text-left">
                      <div class="font-bold text-xl">注册账号</div>
                      <div class="text-sm text-gray-600 mt-3">注册自己的专属账号</div>
                  </div>
              </div>
              <div class="w-full lg:w-4/12 flex items-center mt-6">
                  <div class="w-16 h-16 border-2 border-cus-active rounded-full flex items-center justify-center font-bold number">2</div>
                  <div class="ml-6 text-left">
                      <div class="font-bold text-xl">选择模板</div>
                      <div class="text-sm text-gray-600 mt-3">多模板可供选择</div>
                  </div>
              </div>
              <div class="w-full lg:w-4/12 flex items-center mt-6">
                  <div class="w-16 h-16 border-2 border-cus-active rounded-full flex items-center justify-center font-bold number">3</div>
                  <div class="ml-6 text-left">
                      <div class="font-bold text-xl">下载分享</div>
                      <div class="text-sm text-gray-600 mt-3">轻松下载分享</div>
                  </div>
              </div>
          </div>
      </div>
  </div>

  <!--第五块-->
  <div class="w-full max-w-screen-xl m-auto px-4 lg:px-10 py-20 flex items-center flex-wrap w-full flex-col-reverse lg:flex-row">
      <div class="w-full lg:w-1/2 px-4 lg:px-20">
          <img src="/svg/block-3.svg" class="max-w-sm m-auto">
      </div>
      <div class="w-full lg:w-1/2 lg:pl-10 text-center lg:text-left mb-6 lg:mb-0">
          <h2 class="text-4xl">马上体验，快人一步</h2>
          <div class="mt-8 text-gray-600">即可打开新世界的大门</div>
          <div class="mt-10 flex flex-col lg:flex-row justify-center lg:justify-start">
              <a class="bg-cus-active text-white px-4 py-3 rounded flex items-center justify-center w-48 m-auto lg:ml-0 lg:mr-0" href="/editor" target="_self">
                  <span class="ml-1">
                      免费使用
                  </span>
              </a>
          </div>
      </div>
  </div>

  <!--页面底部页脚-->
  <Footer></Footer>
</template>
