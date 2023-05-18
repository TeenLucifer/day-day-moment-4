<template>
    <div class="flex justify-between w-full py-4 px-4 lg:px-10 items-center fixed top-0">
    <a class="flex h-14 items-center" href="/">
        <img src="/logo.png" class="h-10 lg: lg:h-14"/>
        <span class="ml-2 text-xl font-bold hidden lg:block"></span>
    </a>
    <div class="flex space-x-10 items-center">
        <a href="/" class="hidden lg:block">主页</a>
        <!-- <a href="/guide" class="text-sm lg:text-base">安装教程</a>
        <a href="https://support.qq.com/products/405384" target="_blank" class="text-sm lg:text-base flex items-center">
            问题反馈
        </a> -->
        <a href="/editor" class="hidden lg:block">编辑</a>
        <a href="/sign-in" class="hidden lg:block" >登录</a>
        <a href="/sign-up" class="hidden lg:block" >注册</a>
    </div>
  </div>
</template>
