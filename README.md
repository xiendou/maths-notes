# Math Notes

Personal mathematics notes written in LaTeX, updated as I study.

| Course | LaTeX source | PDF |
| --- | --- | --- |
| Analysis 1 | [Source](0003%20Analysis%201/analysis1.tex) | [Read](0003%20Analysis%201/analysis1.pdf) |
| Algebra 1 | [Source](0005%20Algebra%201/algebra1.tex) | [Read](0005%20Algebra%201/algebra1.pdf) |
| Applied Mathematics 1 | [Source](0008%20Applied%20Mathematics%201/applied-mathematics1.tex) | Not built yet |
| Mathematical Methods 1 | [Source](0010%20Mathematical%20Methods%201/mathematical-methods1.tex) | [Read](0010%20Mathematical%20Methods%201/mathematical-methods1.pdf) |

These are study notes in progress, not official course materials. Some sections
are incomplete; Mathematical Methods includes edited transcriptions of lecture
notes, with source-page references. Original lecture scans are kept locally.

## Build a PDF

Install a LaTeX distribution with XeLaTeX and the packages used by the source.
For example, from the repository root:

```sh
cd "0010 Mathematical Methods 1"
xelatex -interaction=nonstopmode -halt-on-error mathematical-methods1.tex
xelatex -interaction=nonstopmode -halt-on-error mathematical-methods1.tex
```

Run twice so the contents and cross-references update. VS Code with LaTeX
Workshop can also build the notes.

## 保存修改并提交到 GitHub

1. 在 VS Code 中修改笔记并保存；需要更新 PDF 时先编译。
2. 打开左侧 **Source Control（源代码管理）**，查看改动。
3. 点击要提交的文件旁的 **+**，将它们加入本次提交。
4. 写一句说明，例如 `Add notes on orthogonal projection`，然后点击 **Commit**。
5. 点击 **Sync Changes / Push**，将提交上传到 GitHub。

**Commit** 是在本机保存一个有说明的版本；**Push** 才是上传到 GitHub。
可以用中文或英文写提交说明。每完成一个小主题或修正一处错误就提交一次即可。

如果使用终端，例如：

```sh
git add "0005 Algebra 1/algebra1.tex" "0005 Algebra 1/algebra1.pdf"
git commit -m "补充核空间的证明"
git push
```

仓库的 `.gitignore` 默认只允许跟踪上表四个课程文件夹，以及根目录的
README 和 `.gitignore`。LaTeX 临时文件、原讲义扫描件、本地参考备份和
本工作区的其他文件夹均被忽略。
