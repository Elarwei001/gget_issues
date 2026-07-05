# gget issue / PR 分析留档

> 🌐 **在线浏览（渲染版）：https://elarwei001.github.io/gget_issues/** — 点开即是网页，无需下载。

用 [`gget-issue-analysis`](https://github.com/Elarwei001/personal-skills/tree/master/gget-issue-analysis) skill 生成的 gget（scverse/gget）issue / PR 分析报告归档。

每份报告都是**自包含的 HTML**（深色主题、内联 CSS、无外部依赖，右上角可切换中/EN），开头有面向非生物背景读者的背景科普 + 官方链接，随后是"解决什么问题 / 价值 / 数据结构详解 / 如何解决 / 是否契合 gget 平台角色（四 lens 评估）/ live data test 设计 / 当前状态"。

## 报告索引

| PR | 模块 | 一句话 | 在线浏览 |
|----|------|--------|----------|
| [#237](https://github.com/scverse/gget/pull/237) | `gget ref` | 给 `ref` 加 `assembly_report`，把位置参数当 NCBI 装配号、返回跨命名映射表（`chr1↔1↔CM000663.2↔NC_000001.11`） | [🌐 打开](https://elarwei001.github.io/gget_issues/pr237-ref-assembly-report.html) |
| [#238](https://github.com/scverse/gget/pull/238) | `gget ref` | 给 `ref` 加 GENCODE 数据源（人/鼠 GTF+FASTA），与 Ensembl 并列、复用同一返回结构 | [🌐 打开](https://elarwei001.github.io/gget_issues/pr238-ref-gencode.html) |
| [#245](https://github.com/scverse/gget/pull/245) | `gget pineapple` | 接入 Pineapple 策展的生物影像数据集/权重（仅下载，不做图像处理） | [🌐 打开](https://elarwei001.github.io/gget_issues/pr245-pineapple.html) |
| [#242](https://github.com/scverse/gget/pull/242) | `gget mitocarta` | 取 Broad MitoCarta3.0 的两个 `.xls` 线粒体蛋白/通路数据库 | [🌐 打开](https://elarwei001.github.io/gget_issues/pr242-mitocarta.html) |
| [#241](https://github.com/scverse/gget/pull/241) | `gget enrichr` | 给 enrichr 加检索 gene sets（含 MSigDB 合集），复用 Enrichr 端点、返回 tidy 长表 | [🌐 打开](https://elarwei001.github.io/gget_issues/pr241-enrichr.html) |

## 查看方式

- **在线（推荐）**：点上表"🌐 打开"，或直接访问 **https://elarwei001.github.io/gget_issues/** （GitHub Pages 渲染版）。
- 在 GitHub 仓库里直接点 `.html` 文件看到的是**源码**；下载到本地用浏览器打开也能看到渲染效果。

## 命名约定

`pr<编号>-<模块名>.html`，例如 `pr242-mitocarta.html`。新增报告后在上表加一行。
