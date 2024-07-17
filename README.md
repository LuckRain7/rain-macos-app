# rain-macos-app

<p align="center">一个基于Tauri、Vite 5、Vue 3 和 TypeScript 构建的测试项目</p>

<div align="center">
  <img src="https://img.shields.io/badge/TypeScript-blue?logo=Typescript&style=flat&logoColor=fff">
  <img src="https://img.shields.io/badge/Vue3-35495E?logo=vue.js&logoColor=4FC08D">
  <img src="https://img.shields.io/badge/Tauri-24C8DB?logo=tauri&logoColor=FFC131">
  <img src="https://img.shields.io/badge/Rust-c57c54?logo=rust&logoColor=E34F26">
  <img src="https://img.shields.io/badge/Vite5-35495E?logo=vite&logoColor=41D1FF">
  <img src="https://img.shields.io/badge/UnoCss-efefef?logo=UnoCss&logoColor=606060">
  <img src="https://img.shields.io/badge/pnpm-909090?logo=pnpm&logoColor=FFC131">
  <img src="https://img.shields.io/badge/Sass-CC6699?logo=sass&logoColor=fff">
  <img src="https://img.shields.io/badge/Design-Naive-059669">
  <img src="https://img.shields.io/badge/yarn-white?logo=yarn&logoColor=2C8EBB">
</div>

## 项目介绍

rain-macos-app 是一个基于 Tauri、Vite 5、Vue 3 和 TypeScript 构建的测试项目。它利用了 Tauri 的跨平台能力和 Vue 3 的响应式设计，结合了 TypeScript 的类型安全特性和 Vite 5 的快速构建，为用户提供了一个高效、安全和易用的通讯解决方案。

## 技术栈

* **Tauri**: 为本项目提供了一个轻量级的、高性能的桌面应用容器，使得我们可以使用前端技术栈来开发跨平台的桌面应用。Tauri 的设计哲学是在保证安全性的前提下，尽可能减少资源占用。
* **Vite 5**: Vite 是一个现代化的前端构建工具，它利用原生 ES 模块导入的能力来提供一个快速的开发服务器，与此同时，它也为生产环境打包提供了强大的支持。Vite 5 是其最新的版本，带来了更多的优化和特性。
* **Vue 3**: Vue 3 是一个渐进式JavaScript框架，用于构建用户界面。它的组合式API、更好的TypeScript集成和对移动端的优化使得开发复杂的单页应用变得更加简单和高效。
* **TypeScript**: TypeScript 是 JavaScript 的一个超集，它在 JavaScript 的基础上增加了类型系统。这让我们能够在开发过程中捕获更多的错误，并且提供更好的编辑器支持。

## 环境

我们以 macOS 为例：

**1. 首先安装 Xcode 命令行工具**

在终端中执行以下命令：

```bash
bash

 代码解读
复制代码xcode-select --install
```

如果已经安装过 Xcode 命令行工具，则可以直接进行下一步。

**2. 安装 Rust**

在 macOS 上安装 Rust，请打开终端并输入以下命令：

```bash
bash

 代码解读
复制代码curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
```

安装成功后，终端将显示以下内容：

```
Rust is installed now. Great!
```

请确保重新启动终端以使更改生效。

作者：虾卡拉卡
链接：https://juejin.cn/post/7388842078798823433
来源：稀土掘金
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

## 创建项目

Tauri 官方提供了多种项目模板，可以快速搭建项目：

```bash
# pnpm
pnpm create tauri-app

# npm
npm create tauri-app

# yarn
yarn create tauri-app
```

按照提示选择自己喜欢的模板。

这里我们选择 `react` 开发前端页面。

一路回车后，打开项目文件夹。执行安装依赖命令： `pnpm i` 。依赖安装完成后，执行 `pnpm tauri dev` 命令启动项目。这时便会启动一个应用，如下图所示：

## 开发

```bash
# 查看环境及依赖安装情况
npm run tauri info
# 开发启动
npm run tauri dev
# 编译并打包
npm run tauri build
# 打包后目录
/src-tauri/target/release/bundle/dmg
/src-tauri/target/release/bundle/macos
```
