# CBU-DSSAN | 五语言科研展示网站 / Multilingual research project page

## 快速使用 / Quick start

1. 解压网站 ZIP。Unzip the archive.
2. 打开 `index.html`。Open `index.html` in a modern browser to use it offline.
3. 在顶部语言切换器中选择 **中文 / English / Русский / Français / العربية**。
4. 若部署到 GitHub Pages，请将 `index.html`、`assets/`、`images/`、`CBU-DSSAN.pdf` 和 `S1474034622001835.bib` 一起上传到站点根目录。For GitHub Pages, publish these files together in the selected Pages directory.

无需 Node.js、构建命令或第三方前端框架。No build step or third-party frontend framework is required. The content, styles, scripts, illustrations, PDF, and BibTeX are local resources.

## 本次改版 / Features

- 参考 paper2anything 的清晰层级、学术项目主页与响应式设计理念，但自行重建了视觉排版；没有复制该站点素材或代码。
- 深蓝科技主题搭配浅色阅读区；主要研究正文采用两端对齐与更宽松的行距。
- 原始 9 张科研插图和 3 张 HTML 统计表完整保留；插图等比例缩放并支持点击放大。
- 五种语言覆盖研究背景、技术步骤、方法说明、数据表标题与列名、结果解释、局限性、图注及交互提示。
- 阿拉伯语界面使用 `dir="rtl"`，但数据表和科学数值保持 LTR 阅读方向。
- 手机视图支持响应式导航，宽表格可独立横向滚动。
- 三类召回率（TNR / TER / TTR）原始对比图可以切换。
- BibTeX 提供原文显示、精确复制和附件下载。

## 正式引用 / Official citation

**Highly imbalanced fault diagnosis of gas turbines via clustering-based downsampling and deep siamese self-attention network**

Dan Liu, Shisheng Zhong, Lin Lin, Minghang Zhao, Xuyun Fu, Xueyun Liu. *Advanced Engineering Informatics*, 54 (2022), 101725.

DOI: https://doi.org/10.1016/j.aei.2022.101725

**IMPORTANT:** `S1474034622001835.bib` is a byte-identical copy of the second uploaded attachment. The webpage's visible BibTeX text is identical to that file, including its citation key, fields, keywords, and abstract. The formal article refers to **CBU-DSSAN**, although the source ZIP folder was named `CBD-DSSAN_html`.

## 主要文件 / Contents

```text
index.html
assets/style.css
assets/app.js
assets/locales.js
assets/favicon.svg
images/fig1-concept.jpg ... images/fig9-tsne.jpg
CBU-DSSAN.pdf
S1474034622001835.bib
previews/Top_*.png
previews/MobileTop_*.png
previews/Desktop_*.png
previews/Mobile_*.png
previews/qa_report.json
```

## 翻译与科研边界 / Translation and research fidelity

- The original research figure text remains in its source language because the figures are unchanged images.
- All numerical values and comparison results originate from the supplied webpage; the BibTeX originates exclusively from the supplied `.bib` file.
- Russian, French, and Arabic translations should receive a specialist native-language review before broad academic publicity.
- This presentation is an independent research outreach page. The published journal article is the authoritative source.

## 测试 / QA

Browser render QA was carried out for five languages on desktop (1440 × 900) and mobile (390 × 844) layouts, using the same HTML, CSS, JavaScript and image assets in an embedded-resource test page because the test browser restricts local `file://` navigation. The tests confirmed no page-level overflow, no missing rendered figures, no browser script errors, BibTeX string equivalence, mobile navigation, image lightbox and recall-tab interactions.

完整报告：`previews/qa_report.json`
