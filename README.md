<!--
 Copyright (c) 2023 Boshi Yuan
 Copyright (c) 2024 yueneiqi
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

# ECNU Thesis Proposal 华东师大开题报告模板

本仓库是华东师范大学开题报告 LaTeX（非官方）模板，基于仓库 [SJTU Thesis Proposal 上海交大开题报告模板](https://github.com/NemoYuan2008/SJTU-Thesis-Proposal) 制作。

2024年更新了新的模版，增加了导师意见一栏，如果使用新版，取消`main.tex`底部的注释即可。

本模板**仅支持 XeTeX 引擎和 UTF-8 编码，请使用 XeLaTeX 编译**。

如果你觉得本仓库有用，请点个 star 支持一下。

## 免责声明

本模板仅为开题报告模板的参考实现，不保证审查老师不提意见。任何由于使用本模板而引起的论文格式审查问题均与本模板作者无关。

## 获取方法

Github 用户点击上方绿色 Code，选择 Download ZIP 下载源码到本地。或者使用 git 克隆本仓库。

## 使用方法

**请仔细阅读 `main.tex` 中的注释，按照注释的提示进行文档的编写。**

## 编译方法

这里以 Overleaf 和 VSCode 为例说明。注意如果在本地使用需安装最新版 TeXLive 套装。使用其他编辑器的用户可参考相应编辑器的使用说明，只需注意将编译器设置为 XeLaTeX 即可。

### Overleaf 用户

可将从 GitHub 下载下来的压缩包上传至 Overleaf 平台，并将编译器设置为 XeLaTeX。

设置编译器的方法请参见 [Overleaf 官方文档](https://www.overleaf.com/learn/how-to/Changing_compiler)。

### 本地 VSCode 用户

安装 LaTeX Workshop 插件，使用 VSCode 打开文件夹，打开 `main.tex`，选择 `Recipe: latexmk (xelatex)` 进行编译。
在 VSCode 设置中搜索 `latex-workshop.latex.recipe.default` 并将其改为 `lastUsed` 以便一直使用该选项编译。
注意，使用其他选项会导致报错。

### 从命令行编译

使用 `latexmk -xelatex main` 命令来进行编译，可以加入 `-synctex=1` 命令行选项来方便编辑器定位。

如果你熟悉 LaTeX 编译流程也可手动进行编译 `xelatex main && biber main && xelatex main  && xelatex main`，注意文献管理使用的是 `biber` 而不是 `bibtex`。

## 贡献

本模板可能存在一些问题，同时学校提供的官方 word 模板可能随时会更新。如果你发现了模板的问题，欢迎给我发 PR 或者提 issue。

## 许可证

SimSun字体（`SimSun.ttc`）是由北京中易中标电子信息技术有限公司设计的，版权属于中易电子公司（ZHONGYI Electronic Co., 2001年），本仓库用于非商业用途。

其余部分使用 MIT 许可证授权。
