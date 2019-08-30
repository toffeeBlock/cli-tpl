## eo-cli
极简的脚手架生成器demo，实现了核心功能

* 1. 根据package.json 中 bin指定的cli，全局暴露eo-cli
* 2. 根据用户选择，生成自定义的项目名称，简介，创建项目
* 3. templates.json 文件中 path 指向了 vue 脚手架的项目仓库，用户init后，等，动态download该仓库中存放的脚手架

### 部署步骤
```bash
# 全局安装 cli
npm install eo-cli -g

# 初始化脚手架
eo-cli init

# 指定项目名 介绍 作者
```
### 目录结构
```
├── README.md                   // help
├── bin                         // bin目录
│   ├── iyiou-cli               // 定义终端，执行相关命令
├── commands                    // 命令
│   ├── init.js                 // 初始化操作，用户进行交互式的download
├── package.json                // 配置项
└── templates.json              // 配置脚手架git远程仓库地址
```