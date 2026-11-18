# BW-8200C UI 设计预览

1280 × 800 血液回收机交互原型，包含 35 个页面／状态和 16 个报警弹窗。

- [全部界面](新版UI/设计总览.html)
- [直接进入主界面](新版UI/index.html)
- [调试界面](新版UI/index.html?screen=debug)
- [调试参数二级界面](新版UI/index.html?screen=debugDetail)
- [可编辑 Figma 设计稿](https://www.figma.com/design/2mgAGS0RgqawBxkw36RPHs)

## 部署

这是无需构建的静态网页。GitHub Pages 设置为 Deploy from a branch，选择 main 分支和 /(root) 目录。

页面使用相对路径，可部署到仓库子路径。`.nojekyll` 保留原文件结构。网站首页进入设计总览，可切换全部界面、报警状态和旧版对照。

## 本地预览

在仓库根目录运行 `python3 -m http.server 8080`，浏览器访问 `http://localhost:8080`。

## 运行范围

此版本为界面设计与交互预览，尚未接入设备控制。未提供的设备读数显示占位，患者输入只在当前浏览器页面内临时使用。

## 文件

- `新版UI/`：界面代码与必要的品牌／操作照片素材。
- `旧版参考/`：设计总览中的旧版对照图。

设计源文件、验收记录与完整交付包保留在本地项目中。
