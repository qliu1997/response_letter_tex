# Response Letter LaTeX Template

学术论文审稿回复信 LaTeX 模板，支持审稿意见引用与交叉引用。

## 文件说明

| 文件 | 说明 |
|------|------|
| `blank_response_template.tex` | 空白模板，直接填入内容使用 |
| `blank_response_template.pdf` | 空白模板编译结果 |
| `template_guide_zh.tex` | 带详细注释的示例模板（含完整回复示例） |
| `template_guide_zh.pdf` | 示例模板编译结果 |
| `*.refcheck` | 参考文献检查文件 |

## 使用方法

1. 复制 `blank_response_template.tex` 为你的响应文件
2. 修改模板中的占位符内容
3. 使用 XeLaTeX 编译

```bash
xelatex blank_response_template.tex
```

## 模板结构

- `\defref{label}{text}` — 定义审稿意见引用
- `\rcite{label}` — 在正文中引用已定义的审稿意见（蓝色加粗）
- `\section{}` — 审稿意见编号（加粗）
- `\subsection{}` — 审稿意见内容（斜体）

## 编译依赖

- XeLaTeX
- ctexart document class
- geometry, fancyhdr, titlesec, xcolor, setspace 等宏包