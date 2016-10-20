# linux-dash 的汉化版
#### 原地址: https://github.com/afaqurk/linux-dash
---
<br/>
<h1 align="center">
  linux-dash-zh
</h1>

<p align="center">
  Linux Dash是一个基于 Web 的 dashboard, 它看起来简洁、清爽， 可用来监视 Linux 服务器信息。通过 linux-dash，你可以实时、按需监 视CPU、内存、负载、网络、磁盘、用户等许多系统状况。
</p>

<p align="center">
<small>Linux Dash Docs <a href="https://linux-dash.github.io/docs/#getting-started">Linux Dash v2.0</a>: in Fall 2016.</small>
</p>

<p align="center">
  <strong>
    <a href="#"><i>Demo</i></a> &nbsp;|&nbsp;
    <a href="#特性"><i>特性</i></a> &nbsp;|&nbsp;
    <a href="#安装">
      <i>安装</i></a> &nbsp;|&nbsp;
    <a href="#支持"><i>支持</i></a>
  </strong>
</p>

<p align="center">
  <a href="https://github.com/NoBey/linux-dash-zh">
    <img
      width="80%"
      src="./linux-dash.png"
      alt="Linux Dash 中文版">
  </a>
</p>

<br/>

<p align="center">
  <a href="https://github.com/NoBey/linux-dash-zh">
    <img
      width="80%"
      alt="Linux Dash screenshot"
      src="http://i.imgur.com/tehGyrQ.gif">
  </a>
</p>

<br/>
<p align="center">
  <a href="https://github.com/NoBey/linux-dash-zh">
    <img
      src="https://badges.gitter.im/gitterHQ/gitter.png"
      alt="Linux Dash Gitter chat">
  </a>
</p>
## 特性
* 一个漂亮, 简单的基于web的linux服务器监控面板
* 仅仅只需要1MB *(.git removed)*
* 实时数据可视化更新, 可刷新, 和不断添加的模块
* 支持在PHP, Node.js, Python, 和 Go 下安装

## 安装

#### 第一步 : 下载 Linux Dash

克隆 git 项目
```sh
# 中文版
git clone https://github.com/NoBey/linux-dash-zh.git
# 原版 地址
git clone https://github.com/afaqurk/linux-dash.git
```
下载地址 : **[中文版](https://codeload.github.com/NoBey/linux-dash-zh/zip/master)** -
 **[原版](https://github.com/afaqurk/linux-dash/archive/master.zip)**

#### 第二步: 关于Linux Dash的安全问题

Linux Dash 没有任何安全或身份验证功能

**强烈建议** 在Linux Dash 的基础上添加安全措施保护

#### 第三步: 启动 Linux Dash
<h6 align="center">
Linux Dash 能够运行在: <u>Node.js</u>, PHP, Go, 和 Python.
<br/>
<sub>
* 推荐使用 `Node.js` 因为它原生就支持`websockets`和 高性能的 `I/O`操作.
</sub>
</h6>

首先下载或克隆 `linux-dash`然后,参考部分为你的环境:
##### Node.js

NPM 安装依赖文件
```
npm install
```

启动 Linux Dash
```
node server/
```

默认端口是80 需要改变端口去 `server/index.js` 的文件修改端口号.

<br/>
##### PHP
1. 启动你的 `exec`, `shell_exec`, 和 `escapeshellarg` 功能模块
2. 重启你的web服务器 (Apache, nginx, etc.)
  - For PHP + Apache setup follow the [Digital Ocean tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-linux-dash-on-ubuntu-14-04).
  - For help with nginx setup, see [this gist](https://gist.github.com/sergeifilippov/8909839) by [@sergeifilippov](https://github.com/sergeifilippov).

<br/>
##### Go
进入 `linux-dash/server` 的目录 并运行
```
go run index.go
```

To build a binary, run `go build && ./server -h`. See [@tehbilly](https://github.com/sergeifilippov)'s notes [here](https://github.com/afaqurk/linux-dash/pull/281) for binary usage options

##### Python
运行 `./python-server.py` 默认端口是80 需要改变端口去 `python-server.py ` 的文件修改端口号.

## 支持

有问题请提 `issues`
