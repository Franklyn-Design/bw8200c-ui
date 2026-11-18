# BW-8200C UI 设计预览

1280 × 800 血液回收机交互原型，包含 35 个页面／状态和 16 个报警弹窗。

- [全部界面](新版UI/设计总览.html)
- [直接进入主界面](新版UI/index.html)
- [调试界面](新版UI/index.html?screen=debug)
- [调试参数二级界面](新版UI/index.html?screen=debugDetail)
- [可编辑 Figma 设计稿](https://www.figma.com/design/2mgAGS0RgqawBxkw36RPHs)

## Cloudflare Pages 部署

连接 GitHub 仓库 `Franklyn-Design/bw8200c-ui`，使用以下设置：

| 设置 | 值 |
| --- | --- |
| 项目名称 | `bw8200c-ui` |
| 生产分支 | `main` |
| 框架预设 | `None` |
| 构建命令 | `exit 0` |
| 构建输出目录 | `.` |
| 根目录（高级） | 留空，使用仓库根目录 |
| 环境变量 | 无需添加 |

保存并部署后，使用 Cloudflare 实际分配的 `*.pages.dev` 默认域名。连接仓库后，后续推送到 main 会自动发布。

这是无需构建的静态网页，根目录已有 index.html。所有界面、操作照片和旧版对照图都在仓库内，不依赖 GitHub 的运行时资源请求。

[Cloudflare 静态 HTML 部署文档](https://developers.cloudflare.com/pages/framework-guides/deploy-anything/)

## 本地预览

在仓库根目录运行 `python3 -m http.server 8080`，浏览器访问 `http://localhost:8080`。

## 运行范围

此版本为界面设计与交互预览，尚未接入设备控制。未提供的设备读数显示占位，患者输入只在当前浏览器页面内临时使用。

## 文件

- `新版UI/`：界面代码与必要的品牌／操作照片素材。
- `旧版参考/`：设计总览中的旧版对照图。

设计源文件、验收记录与完整交付包保留在本地项目中。

