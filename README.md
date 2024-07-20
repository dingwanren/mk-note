# 静态笔记

- 学会用 github page 部署
- 了解如何用 vueuse
  vueuse 是基于组合式 api 的,虽然可以在 vue2 中用,但也是得先用 @vue/composition-api 将选项式变为组合式

- 手动创建项目
  1. npm init
  2. git init, 创建 .gitignore 来指定 git 忽略的文件或目录
  3. 安装依赖,我直接参考文档中 (Vite + Vue 3)[https://github.com/vueuse/vueuse-vite-starter] 的 package.json, cv 一份后, npm install进行安装
  4. 创建 src 目录,index.html, main.js, App.vue
  5. main.js 引入 vue, App.vue, 通过 createApp 创建 vue 应用,挂载到index.html #app 的 div 上(这些应该是 vite 帮忙做的,可去了解过程)
  6. 配置 vite.config.js, 不使用 @vitejs/plugin-vue,将无法解析 App.vue
  7. 访问 yarn dev 的本地服务器,即可看见 App.vue 的内容