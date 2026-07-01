# gget issue / PR 分析留档

用 [`gget-issue-analysis`](https://github.com/Elarwei001/personal-skills/tree/master/gget-issue-analysis) skill 生成的 gget（scverse/gget）issue / PR 分析报告归档。

每份报告都是**自包含的 HTML**（深色主题、内联 CSS、无外部依赖），开头有面向非生物背景读者的背景科普 + 官方链接，随后是"解决什么问题 / 价值 / 如何解决 / 是否契合 gget 平台角色（四 lens 评估）/ live data test 设计 / 当前状态"。

## 报告索引

| PR | 模块 | 一句话 | 报告 |
|----|------|--------|------|
| [#245](https://github.com/scverse/gget/pull/245) | `gget pineapple` | 接入 Pineapple 策展的生物影像数据集/权重（仅下载，不做图像处理） | [pr245-pineapple.html](./pr245-pineapple.html) |
| [#242](https://github.com/scverse/gget/pull/242) | `gget mitocarta` | 取 Broad MitoCarta3.0 的两个 `.xls` 线粒体蛋白/通路数据库 | [pr242-mitocarta.html](./pr242-mitocarta.html) |

## 查看方式

- GitHub 上直接点开是 HTML 源码；**下载到本地用浏览器打开**即可看到渲染效果。
- 或对本 repo 开启 **GitHub Pages**（Settings → Pages → main / root），即可在线渲染浏览。

## 命名约定

`pr<编号>-<模块名>.html`，例如 `pr242-mitocarta.html`。
