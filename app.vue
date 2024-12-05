<!--
* @FileDescription: nuxt项目入口文件
* @Author: Jintao Wang
* @Date: 2024-12-05
* @LastEditors: Jintao Wang
* @LastEditTime: 2024-12-05
-->

<!--
* added by wangjintao
* vue文件编写的一些规范
* 1. 缩进使用两个空格
* 2. vue文件全局注释和<template></template>标签内注释标签看本条注释的使用
* 3. <script></script>标签内部多行注释用 /* */, 单行注释用//
* 4. <style></style>标签内部多行注释和单行注释都用 /* */
-->
<style>
  /*
  :root选择器
  定义了一个CSS变量--el-color-primary, 并使用!important确保优先级最高
  这个变量可以在全局使用
  */
  :root {
    --el-color-primary: rgb(235, 69, 95) !important;
  }
  /*
  .transition-light类
  定义了一个过渡效果, 应用于所有属性, 持续时间为0.3s, 运动曲线为cubic-bezier(0.645, 0.045, 0.355, 1)
  */
  .transition-light {
      transition: all 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);
  }
  /*
  .scroll_conten_auto类
  定义了自定义滚动条的样式。
  ::-webkit-scrollbar 选择器设置滚动条的宽度和高度。
  ::-webkit-scrollbar-track 选择器设置滚动条轨道的背景和圆角。
  ::-webkit-scrollbar-thumb 选择器设置滚动条拇指的背景和圆角。
  */
  .scroll_content_auto::-webkit-scrollbar {
      width: 7px;
      height: 10px;
  }
  .scroll_content_auto::-webkit-scrollbar-track {
      background: transparent;
      border-radius: 2px;
  }
  .scroll_content_auto::-webkit-scrollbar-thumb {
      background: #bfbfbf;
      border-radius: 7px;
  }
  /* 上面定义的全局样式在整个应用程序中都可以使用, 无需在每个组件中重复定义 */
</style>

<!--
  在Nuxt.js项目中，`app.vue`文件通过`<NuxtPage />`组件来启动和渲染首页。具体流程如下：
  1. **项目启动**：
    当你运行`npm run dev`或`npm start`命令时，Nuxt.js会启动开发服务器或生产服务器。
  2. **加载配置**：
    Nuxt.js会读取`nuxt.config.ts`文件中的配置，加载所需的模块和插件。
  3. **渲染`app.vue`**：
    Nuxt.js会首先渲染`app.vue`文件。这个文件定义了全局的样式和布局，并包含一个`<NuxtPage />`组件。
  4. **渲染首页**：
    `<NuxtPage />`组件会根据当前的路由渲染对应的页面组件。当用户访问首页（即`/`路径）时，Nuxt.js会自动渲染`pages/index.vue`文件对应的组件。

  当用户访问`http://localhost:3000/`时，Nuxt.js会渲染`pages/index.vue`中的内容，并将其插入到`<NuxtPage />`组件的位置。
  总结来说，`app.vue`通过`<NuxtPage />`组件来启动和渲染首页，而`<NuxtPage />`组件会根据当前路由自动加载和渲染对应的页面组件。
-->
<template>
  <NuxtPage />
</template>