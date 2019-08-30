## eo-cli
企业级脚手架

### 项目架构

#### webpack4 + vue + vuex + vue-router 搭建前后端分离项目

### 部署步骤
```
1. npm install eo-cli -g
2. eo-cli init
```
### 目录结构
```
├── Readme.md                   // help
├── build                       // 配置
│   ├── webpack.base.config.js  // 开发环境和生产环境公用配置文件
│   ├── webpack.dev.config.js   // 开发环境配置
│   ├── webpack.dll.config.js   // 生产环境打包公共资源
│   ├── webpack.prod.config.js  // 生产环境配置
├── config                      // 配置
│   ├── index.js                // api baseURL 配置 及 开发环境下跨域代理 proxy 配置
├── package.json
├── public                      // 开发环境主目录
│   ├── api                     // 所有请求
│   ├── assets                  // 静态资源文件
│       ├── css                 // 样式文件
│       ├── images              // 图片资源
│   ├── components              // 组件
│   ├── layout                  // 全局Layout组件
│   ├── router                  // 前端路由配置
│   ├── store                   // 状态管理
│   ├── util                    // 公用方法
│   ├── views                   // vue页面
│   ├── App.vue                 // 根vue文件
│   ├── index.html              // 入口页面
│   ├── main.js                 // 入口文件
├── .babelrc                    // babel配置
├── postcss.config.js           // postcss配置
└── tools
```