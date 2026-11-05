# Mathematical Methods 1

日常编辑和编译的文件是 **`mathematical-methods1.tex`**。全部笔记都在这一个文件里，按下面的顺序排列，没有拆成多个章节文件：

1. Chapter 1 — Vectors
2. Chapter 2 — Complex Numbers
3. Chapter 3 — Differential Calculus

在 VS Code 中搜索 `\chapter{` 可以跳到各章；每章内部使用 `\section` 和 `\subsection`。正文使用英文，方便与教授的讲义对照。各章末尾的注释区可以加入自己的解释和改写。

## 原始讲义与章节对应

以下原始扫描讲义保留在本机，未包含在公开仓库中；表格用于说明笔记来源。

| 原始文件 | 内容所在位置 |
| --- | --- |
| `Slides-Week_1.pdf`，14 页 | Chapter 1：向量的几何定义、运算、坐标、直线、点积和平面 |
| `Slides_Week-2.pdf`，15 页 | Chapter 1：投影、叉积、三重积和指标记号 |
| `Slides_Week-3.pdf`，PDF 第 1–6 页 | Chapter 1 续讲：指标记号、向量三重积推导，以及平面与距离例题 |
| `Slides_Week-3.pdf`，PDF 第 7–17 页 | Chapter 2：复数；原手写页码 34–44 |
| `Slides_Week-4.pdf`，19 页 | Chapter 3：导数、反函数、隐式求导、应用、积分和级数；原手写页码 44–62 |

正文小节旁标的是原手写页码；标注 `PDF pp.` 时指 PDF 中的实际页面。不同文件的手写页码有重复，核对时应同时看文件名。Week 2 末尾与 Week 3 开头重复的 recap 已合并，同一段推导只保留一次。积分和级数仍放在 Chapter 3，因为教授这份讲义就是这样安排的。

## 整理方式

- 按教授的原始笔记整理正文、定义、公式、推导、证明思路和例题解答，不使用旧参考版中另外编写的题目代替教授例题。
- 向量统一用粗体代替手写下划线；关键示意图以 LaTeX 重绘，不是扫描图逐笔复刻。
- 补明公式必要的适用条件，例如反函数求导时分母非零、积分幂公式中的指数不等于 −1，以及 Taylor 多项式与无穷级数相等的区别。
- 教授留作练习的二阶近似题保留为练习，并保留讲义边注中的近似数值。

## 原来的按周参考版

原先那份按 Week 1–10 写好的完整参考笔记已原样保存在：

- `reference/weekly-companion-original.tex`
- `reference/weekly-companion-original.pdf`

它是之前独立编写的学习参考资料，与现在基于教授前四周原稿整理的主文件分开保留。`reference/` 仅作为本地备份，不上传公开仓库。

## 编译

在当前本地工作区中，保存主文件会触发现有的 LaTeX Workshop 构建。运行 **LaTeX Workshop: View LaTeX PDF file** 查看同目录的 `mathematical-methods1.pdf`。本机的 VS Code 配置不包含在公开仓库中；克隆到其他电脑后也可以在本目录运行两次 `xelatex mathematical-methods1.tex`。
