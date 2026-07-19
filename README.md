# 吴恩达机器学习笔记

这是一份使用 LaTeX 编写的中文机器学习学习笔记，当前内容涵盖机器学习的基本分类、监督学习与非监督学习、单变量线性回归、代价函数以及批量梯度下降。

本仓库是个人学习记录，并非吴恩达课程或相关平台的官方资料。

## 在线阅读

- [第一周笔记 PDF](output/pdf/thefirstweek.pdf)
- [第一周 LaTeX 源码](thefirstweek.tex)

## 当前内容

- 机器学习的定义与主要类型
- 监督学习中的回归与分类
- 非监督学习中的聚类、异常检测与降维
- 单变量线性回归模型 $f_{w,b}(x)=wx+b$
- 均方误差代价函数 $J(w,b)$
- $J(w,b)$ 的二维梯度与批量梯度下降
- 参数同时更新与顺序更新的区别

## 仓库结构

```text
.
|-- thefirstweek.tex              # 第一周笔记源码
|-- output/
|   `-- pdf/
|       `-- thefirstweek.pdf      # 可直接阅读的 PDF
|-- templates/
|   `-- notebook-template.tex     # 笔记排版模板示例
|-- .vscode/
|   `-- settings.json             # LaTeX Workshop 配置
|-- .gitignore
|-- LICENSE
`-- README.md
```

`build/` 用于存放本地编译产生的中间文件，不纳入版本控制。

## 本地编译

请安装较新的 TeX Live，并确保 `latexmk` 和 `xelatex` 已加入 `PATH`。在仓库根目录运行：

```powershell
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build thefirstweek.tex
```

编译结果位于 `build/thefirstweek.pdf`。提交内容前，可将最新 PDF 更新到公开文档目录：

```powershell
Copy-Item build/thefirstweek.pdf output/pdf/thefirstweek.pdf
```

使用 VS Code 时，安装 LaTeX Workshop 扩展后打开 `.tex` 文件即可按仓库配置自动编译。

## 许可证与说明

本仓库中原创的笔记源码与排版代码采用 [MIT License](LICENSE) 发布。课程名称、课程内容以及可能引用的第三方材料，其权利仍归各自权利人所有。
