# fish_data
DATA BACKUP
ADAPT FISH TO ALL VERSION

DOWNLOAD:
https://asdqp.lanzout.com/b08trrqve
PW:0000

# This project is no longer updated and has been adapted to most possible future versions

# 🧩 修改 APK 教程

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-Android-green.svg)
![Tool](https://img.shields.io/badge/tool-MT_Manager-orange.svg)

---

## 📘 目录

* [🔹 第一步：Fork 本仓库](#-第一步fork-本仓库)
* [🔹 第二步：下载原始 APK](#-第二步下载原始-apk)
* [🔹 第三步：反编译 APK](#-第三步反编译-apk)
* [🔹 第四步：修改内容](#-第四步修改内容)
* [🔹 第五步：回编译并签名](#-第五步回编译并签名)
* [⚠️ 安装提示](#️-安装提示)
* [✅ 完成！](#-完成)

---

## 🔹 第一步：Fork 本仓库

1. 打开本项目的 GitHub 页面
2. 点击右上角的 **Fork** 按钮，将仓库复制到你的账户下
3. 这样你将拥有一个属于自己的副本，用于存放自定义文件

> 📎 你可以在 Fork 后的仓库中自由修改和上传文件

---

## 🔹 第二步：下载原始 APK

下载以下文件并保存到你的设备：

```
1.4.0_7.15_sub.apk
```

（你可以在本项目的 **Releases** 页面找到此文件）

---

## 🔹 第三步：反编译 APK

使用任意反编译工具打开 APK，推荐使用 **MT 管理器**：

1. 打开 MT 管理器
2. 找到并选中 `1.4.0_7.15_sub.apk`
3. 选择 **“反编译（Dex 编辑器）”** 或 **“Dex 编辑器+”**
4. 打开并加载 `classes.dex` 文件

---

## 🔹 第四步：修改内容

在 `classes.dex` 文件中搜索并替换内容：

### 🔍 搜索以下字符串：

```
https://fish.enlysure.com
```

### ✏️ 替换为：

```
https://github.com/你的用户名/你的仓库名/raw/master
```

#### ✅ 示例：

```
https://github.com/Eli-Fourier/fish-apk/raw/master
```

> ⚠️ 注意：
>
> * 请确保你的仓库为 **公开（Public）**，否则 APK 无法访问资源
> * 替换时保持 **https://** 与路径格式完整一致

---

## 🔹 第五步：回编译并签名

修改完成后，需要重新打包并签名 APK。

### 方法一：使用 MT 管理器签名（推荐）

1. 回编译 APK
2. 打开编译好的新 APK 文件
3. 选择 **签名** 功能（MT 自带签名工具）
4. 安装签名后的 APK

### 方法二：命令行签名（可选）

```bash
# 使用 apksigner 工具签名示例
apksigner sign --ks mykey.keystore --out app-signed.apk app-unsigned.apk
```

---

## ⚠️ 安装提示

* 若安装失败，请 **先卸载旧版本** 再安装新 APK
* 签名必须一致，否则系统会提示签名冲突
* 若仍有问题，可尝试清除缓存或使用不同包名重新签名

---

## ✅ 完成！

🎉 恭喜！
你现在的 APK 已成功指向你自己的 GitHub 仓库地址。

> 💡 之后只需更新你仓库中的文件，APK 就会自动加载最新内容。

---

**Made with ❤️ by [Eli Fourier](https://github.com/Eli-Fourier)**
