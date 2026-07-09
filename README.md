# gget issue / PR 分析留档

> 🌐 **在线浏览（渲染版）：https://elarwei001.github.io/gget_issues/** — 点开即是网页，无需下载。

用 [`gget-issue-analysis`](https://github.com/Elarwei001/personal-skills/tree/master/gget-issue-analysis) skill 生成的 gget（scverse/gget）issue / PR 分析报告归档。

每份报告都是**自包含的 HTML**（深色主题、内联 CSS、无外部依赖，右上角可切换中/EN），开头有面向非生物背景读者的背景科普 + 官方链接，随后是"解决什么问题 / 价值 / 数据结构详解 / 如何解决 / 是否契合 gget 平台角色（四 lens 评估）/ live data test 设计 / 当前状态"。

## 报告索引

| PR | 模块 | 一句话 | 在线浏览 |
|----|------|--------|----------|
| [#232](https://github.com/scverse/gget/pull/232) | `gget alliance` | 新模块：包装 Alliance of Genome Resources REST API，自动分两种模式（基因 ID→`/gene` 详情；自由词→`/search`，按 category）；PI 点名（#162）；真机探针证实两模式字段 + 全部 6 类 category 映射 + 错误处理都对；含引用顺序/缺西语页/缺 live 测试/坏 category 静默返空等发现 | [🌐 打开](https://elarwei001.github.io/gget_issues/pr232-alliance.html) |
| [#233](https://github.com/scverse/gget/pull/233) | `gget ucsc` | 新模块：包装 UCSC 官方 `/search` REST 端点，「基因名/词条 → UCSC ID + 位置（按轨道分组）」→ DataFrame/json，类比 `gget search`；真机探针证实结构吻合、quirk 处理正确；含引用顺序/缺西语页/坏 genome 报错被吞/缺 live 测试等发现 | [🌐 打开](https://elarwei001.github.io/gget_issues/pr233-ucsc.html) |
| [#235](https://github.com/scverse/gget/pull/235) | `gget alphafold` | 加 `msa` 参数：传自定义 MSA、跳过 jackhmmer 搜索（免下 ~2GB 库）；a3m 解析复现 AlphaFold 原算法、改善可复现性；含 pre-commit 红根因 | [🌐 打开](https://elarwei001.github.io/gget_issues/pr235-alphafold-custom-msa.html) |
| [#236](https://github.com/scverse/gget/pull/236) | `gget reactome` | 新模块：用 Reactome ContentService REST API 做三类查询（通路/搜索/实体），返回 tidy DataFrame；测试设计良好、含 pre-commit 红根因 | [🌐 打开](https://elarwei001.github.io/gget_issues/pr236-reactome.html) |
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
