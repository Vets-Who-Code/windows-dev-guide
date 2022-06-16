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
  - [Mapping Your Linux Drive](#mapping-your-linux-drive)
    - [Pin Your Code Directory](#pin-your-code-directory)
  - [Restarting WSL](#restarting-wsl)
- [👨‍💻 Windows Terminal](#windows-terminal-4)
  - [Installing Windows Terminal](#installing-windows-terminal)
  - [Terminal Settings](#terminal-settings)
    - [Default Profile](#default-profile)
    - [Starting Directory](#starting-directory)
- [📝 Git Config](#-git-config-5)
  - [Name](#name)
  - [Email](#email)
  - [Username](#username)
- [😺 GitHub Credentials](#-github-credentials-6)
  - [Creating your Personal Access Token](#creating-your-personal-access-token)
  - [Git Credential Manager](#git-credential-manager)
  - [Storing Your Token](#storing-your-token)
- [💤 Zsh](#-zsh-7)
  - [Installing Zsh](#installing-zsh)
  - [OhMyZsh](#ohmyzsh)
  - [cURL](#curl)
  - [Installing OhMyZsh](#installing-ohmyzsh)
  - [More Plugins](#more-plugins)
    - [zsh-autosuggestions](#zsh-autosuggestions)
    - [zsh-syntax-highlighting](#zsh-syntax-highlighting)
- [📦 Node.js](#-nodejs-8)
  - [NVM](#nvm)
    - [Installing NVM](#installing-nvm)
    - [Changing Node Version](#changing-node-version)
- [💻 Visual Studio Code](#-visual-studio-code)
  - [Installing VS Code](#installing-vs-code)
  - [Changing the Default Shell](#changing-the-default-shell)
  - [Remote Extension](#remote-extension)
  - [More Extensions](#more-extensions)
- [🍫 Chocolatey](#-chocolatey-9)
  - [Admin Shell](#admin-shell)
    - [Option 1](#option-1)
    - [Option 2](#option-2)
    - [Option 3](#option-3)
  - [Installing Chocolatey](#installing-chocolatey)
  - [Basic Chocolatey Commands](#basic-chocolatey-commands)
  - [Windows Apps](#windows-apps)
- [🪜 Chrome Extensions](#-chrome-extensions)
- [🇺🇸 VetsWhoCode Web App](#-vetswhocode-web-app)
- [➕ Extracurriculars](

## 🔭 概述

经过大量的试验好错误，我已经能够平凑出一个相当令人满意的Windows开发环境。网络上已经有了很多教程指南，但似乎没有一个涵盖整个范围的，我相信这篇文章会给广大用户带来流畅舒适的Windows 开发体验。

<p align="center">
<img src="images/demo.gif" alt="Using wox, windows term, ohmyzsh, and vs code" />
</p>