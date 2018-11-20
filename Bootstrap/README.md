# 1.Bootstrap起步

**参考链接：**[https://v3.bootcss.com/getting-started/](https://v3.bootcss.com/getting-started/)，简要介绍 Bootstrap，以及如何下载、使用，还有基本模版和案例，等等。

**Bootstrap教程|菜鸟教程：**[http://www.runoob.com/bootstrap/bootstrap-tutorial.html](http://www.runoob.com/bootstrap/bootstrap-tutorial.html)

**Bootstrap 官方网站：**[http://getbootstrap.com/](http://getbootstrap.com/)，可以在该站点上找到所有可用的文档和下载。

## 1.1 Bootstrap 包的内容

### 1.1.1 基本结构：

Bootstrap 提供了一个带有网格系统、链接样式、背景的基本结构。这将在 Bootstrap 基本结构 部分详细讲解。

### 1.1.2 CSS：

Bootstrap 自带以下特性：全局的 CSS 设置、定义基本的 HTML 元素样式、可扩展的 class，以及一个先进的网格系统。这将在 Bootstrap CSS 部分详细讲解。

### 1.1.3 组件：

Bootstrap 包含了十几个可重用的组件，用于创建图像、下拉菜单、导航、警告框、弹出框等等。这将在 布局组件 部分详细讲解。

### 1.1.4 JavaScript 插件：

Bootstrap 包含了十几个自定义的 jQuery 插件。您可以直接包含所有的插件，也可以逐个包含这些插件。这将在 Bootstrap 插件 部分详细讲解。

### 1.1.5 定制：

您可以定制 Bootstrap 的组件、LESS 变量和 jQuery 插件来得到您自己的版本。

## 1.2 安装

**参考：**[Bootstrap中文网 Bootstrap3中文文档](https://v3.bootcss.com/)

### 1.2.1 下载 Bootstrap（预编译版）

[v3.3.7下载链接](https://github.com/twbs/bootstrap/releases/download/v3.3.7/bootstrap-3.3.7-dist.zip)

目录结构：
```
bootstrap/
├── css/
│   ├── bootstrap.css
│   ├── bootstrap.css.map
│   ├── bootstrap.min.css
│   ├── bootstrap.min.css.map
│   ├── bootstrap-theme.css
│   ├── bootstrap-theme.css.map
│   ├── bootstrap-theme.min.css
│   └── bootstrap-theme.min.css.map
├── js/
│   ├── bootstrap.js
│   └── bootstrap.min.js
└── fonts/
    ├── glyphicons-halflings-regular.eot
    ├── glyphicons-halflings-regular.svg
    ├── glyphicons-halflings-regular.ttf
    ├── glyphicons-halflings-regular.woff
    └── glyphicons-halflings-regular.woff2
```

### 1.2.2 Bootstrap 源码

[v3.3.7源码下载地址](https://github.com/twbs/bootstrap/archive/v3.3.7.zip)

Bootstrap 源码包含了预先编译的 CSS、JavaScript 和图标字体文件，并且还有 LESS、JavaScript 和文档的源码。具体来说，主要文件组织结构如下：

```
bootstrap/
├── less/
├── js/
├── fonts/
├── dist/
│   ├── css/
│   ├── js/
│   └── fonts/
└── docs/
    └── examples/
```

`less/`、`js/` 和 `fonts/` 目录分别包含了 CSS、JS 和字体图标的源码。`dist/` 目录包含了上面所说的预编译 Bootstrap 包内的所有文件。`docs/` 包含了所有文档的源码文件，`examples/` 目录是 Bootstrap 官方提供的实例工程。除了这些，其他文件还包含 Bootstrap 安装包的定义文件、许可证文件和编译脚本等。

编译方法参考：[https://v3.bootcss.com/getting-started/#grunt](https://v3.bootcss.com/getting-started/#grunt)

### 1.2.3 Bootstrap CDN

使用 BootCDN 提供的免费 CDN 加速服务（同时支持 http 和 https 协议）

```
<!-- 最新版本的 Bootstrap 核心 CSS 文件 -->
<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

<!-- 可选的 Bootstrap 主题文件（一般不用引入） -->
<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">

<!-- 最新的 Bootstrap 核心 JavaScript 文件 -->
<script src="https://cdn.bootcss.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
```


国内推荐使用 BootCDN 上的库：

```
<!-- 新 Bootstrap 核心 CSS 文件 -->
<link href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">

<!-- 可选的Bootstrap主题文件（一般不使用） -->
<script src="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap-theme.min.css"></script>

<!-- jQuery文件。务必在bootstrap.min.js 之前引入 -->
<script src="https://cdn.bootcss.com/jquery/2.1.1/jquery.min.js"></script>

<!-- 最新的 Bootstrap 核心 JavaScript 文件 -->
<script src="https://cdn.bootcss.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
```

JavaScript 放置在文档最后面可以使页面加载速度更快，因此可以将jquery.min.js和bootstrap.min.js放置在body部分的最后。CSS仍放在head部分。

### 1.2.4 实例精选

以下实例全部基于前面所讲的基本模板并配合 Bootstrap 的众多组件开发而成。我们鼓励你根据自身项目的需要对 Bootstrap 进行定制和修改。

链接：[https://v3.bootcss.com/getting-started/#examples](https://v3.bootcss.com/getting-started/#examples)

实例可以在源码的`docs/examples/`目录下找到。

# 2.Bootstrap教程

**Bootstrap教程|菜鸟教程：**[http://www.runoob.com/bootstrap/bootstrap-tutorial.html](http://www.runoob.com/bootstrap/bootstrap-tutorial.html)

## 目录

- Bootstrap 教程
    - [Bootstrap 教程](README.md)
    - [Bootstrap 简介](01-02-intro1.html)
    - [Bootstrap 环境安装](01-03-bootstrap-template1.html)
- Bootstrap CSS
    - [Bootstrap CSS 概览](02-01-css-overview.html)
    - [Bootstrap 网格系统](02-02-grid-system-example1-col-md.html)
    - [Bootstrap 排版](#)
    - [Bootstrap 代码](#)
    - [Bootstrap 表格](#)
    - [Bootstrap 表单](#)
    - [Bootstrap 按钮](#)
    - [Bootstrap 图片](#)
    - [Bootstrap 辅助类](#)
    - [Bootstrap 响应式实用工具](#)
- Bootstrap 布局组件
    - [Bootstrap 字体图标](#)
    - [Bootstrap 下拉菜单](#)
    - [Bootstrap 按钮组](#)
    - [Bootstrap 按钮下拉菜单](#)
    - [Bootstrap 输入框组](#)
    - [Bootstrap 导航元素](#)
    - [Bootstrap 导航栏](#)
    - [Bootstrap 面包屑导航](#)
    - [Bootstrap 分页](#)
    - [Bootstrap 标签](#)
    - [Bootstrap 徽章](#)
    - [Bootstrap 超大屏幕](#)
    - [Bootstrap 页面标题](#)
    - [Bootstrap 缩略图](#)
    - [Bootstrap 警告](#)
    - [Bootstrap 进度条](#)
    - [Bootstrap 多媒体对象](#)
    - [Bootstrap 列表组](#)
    - [Bootstrap 面板](#)
    - [Bootstrap Wells](#)
    - [Bootstrap 创建一个网页](#)
- Bootstrap 插件
    - [Bootstrap 插件概览](#)
    - [Bootstrap 过渡效果](#)
    - [Bootstrap 模态框](#)
    - [Bootstrap 下拉菜单](#)
    - [Bootstrap 滚动监听](#)
    - [Bootstrap 标签页](#)
    - [Bootstrap 提示工具](#)
    - [Bootstrap 弹出框](#)
    - [Bootstrap 警告框](#)
    - [Bootstrap 按钮](#)
    - [Bootstrap 折叠](#)
    - [Bootstrap 轮播](#)
    - [Bootstrap 附加导航](#)
- Bootstrap 其他
    - [Bootstrap UI 编辑器](#)
    - [Bootstrap v2 教程](#)
    - [Bootstrap HTML编码规范](#)
    - [Bootstrap CSS编码规范](#)
    - [Bootstrap 可视化布局](#)
    - [Less 教程](#)