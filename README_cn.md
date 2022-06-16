<p align="center">
<img src="images/windows.jpg" alt="Microsoft Windows Logo" width="500px" />
</p>
<h1 align="center">Windows 开发者设置指南(2022)</h1>

[English](./README.md) | 中文 



English | [中文](./README_cn.md)

- [🔭 概述](#-概述)
- [☑ 开始之前](#-开始之前)
- [🐧 WSL](#-wsl-1-2-3)
  - [安装 WSL 2](#安装-wsl-2)
  - [用户配置](#用户配置)
  - [更新Linux](#更新Linux)
  - [映射您的Linux驱动器](#映射您的Linux驱动器)
    - [固定代码目录](#固定代码目录)
  - [重启WSL](#重启WSL)
- [👨‍💻 Windows Terminal](#windows-terminal)
  - [安装 Windows Terminal](#安装 Windows Terminal)
  - [终端设置](#终端设置)
    - [默认配置文件](#默认配置文件)
    - [初始目录](#初始目录)
- [📝 Git Config](#Git Config)
  - [Name](#name)
  - [Email](#email)
  - [Username](#username)
- [😺 GitHub Credentials](#-github-credentials-6)
  - [创建个人token](#创建个人token)
  - [Git管理](#Git管理)
  - [存储token](#存储token)
- [💤 Zsh](#-zsh-7)
  - [安装 Zsh](#安装 Zsh)
  - [OhMyZsh](#ohmyzsh)
  - [cURL](#curl)
  - [安装 OhMyZsh](#安装 ohmyzsh)
  - [更多插件](#more-plugins)
    - [zsh-autosuggestions](#zsh-autosuggestions)
    - [zsh-syntax-highlighting](#zsh-syntax-highlighting)
- [📦 Node.js](#-nodejs-8)
  - [NVM](#nvm)
    - [安装 NVM](#安装 NVM)
    - [更换 Node 版本](#更换 Node 版本)
- [💻 Visual Studio Code](#-visual-studio-code)
  - [安装 VS Code](#安装 vs-code)
  - [更换默认终端](#更换默认终端)
  - [远程拓展](#远程拓展)
  - [更多拓展](#更多拓展)
- [🍫 Chocolatey](#-chocolatey-9)
  - [Admin Shell](#admin-shell)
    - [Option 1](#option-1)
    - [Option 2](#option-2)
    - [Option 3](#option-3)
  - [安装 Chocolatey](#安装 Chocolatey)
  - [基础 Chocolatey 命令](#基础 Chocolatey 命令)
  - [Windows Apps](#windows-apps)
- [🪜 Chrome 拓展](#-chrome 拓展)
- [🇺🇸 VetsWhoCode Web App](#-vetswhocode-web-app)
- [➕ Extracurriculars](

## 🔭 概述

经过大量的试验好错误，我已经能够平凑出一个相当令人满意的Windows开发环境。网络上已经有了很多教程指南，但似乎没有一个涵盖整个范围的，我相信这篇文章会给广大用户带来流畅舒适的Windows 开发体验。

<p align="center">
<img src="images/demo.gif" alt="Using wox, windows term, ohmyzsh, and vs code" />
</p>

## ☑ 开始之前
- Windows 10 version 2004 and higher (Build 19041 and higher) or Windows 11 [(Which version do I have?)](https://support.microsoft.com/en-us/topic/628bec99-476a-2c13-5296-9dd081cdd808)
- 一个 [GitHub](https://github.com) 账户

## 🐧 WSL [^1] [^2] [^3]
设置Windows开发环境的第一个也是最重要的部分是安装Windows Subsystem for Linux（WSL）。我建议坚持使用Ubuntu，但可以随意尝试你喜欢的发行版。同时安装多个发行版是没有问题的。

### 安装-wsl-2

WSL 2是WSL的最新版本，增加了新的功能，如完整的Linux内核和完整的系统调用兼容性。以前安装它需要几个步骤，但现在我们只需要在PowerShell或Command Prompt中输入以下命令即可。

```sh
wsl --install
```

这条命令的作用是：

- 启用可选的WSL和虚拟机平台组件
- 下载并安装最新的Linux内核
- 设置WSL 2为默认值
- 下载并安装Ubuntu Linux发行版（可能需要重新启动）。

使用`--install`命令默认为Ubuntu，只有在WSL还没有安装的情况下才有效。如果你想改变你的默认Linux发行版, [跟着这篇文章](https://docs.microsoft.com/en-us/windows/wsl/install#change-the-default-Linux-distribution-installed).