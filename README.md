# 吴恩达机器学习笔记

这是一份使用 LaTeX 编写的中文机器学习学习笔记。目前内容涵盖机器学习基础、监督学习与非监督学习、线性回归、梯度下降、特征工程、逻辑回归、多类别分类、过拟合与正则化。

本仓库是个人学习记录，并非吴恩达课程或相关平台的官方资料。

## 在线阅读

- [第一周笔记 PDF](output/pdf/thefirstweek.pdf)
- [第一周 LaTeX 源码](thefirstweek.tex)
- [第二周笔记 PDF](output/pdf/thesecondweek.pdf)
- [第二周 LaTeX 源码](thesecondweek.tex)
- [第三周笔记 PDF](output/pdf/thethirdweek.pdf)
- [第三周 LaTeX 源码](thethirdweek.tex)

## 当前内容

### 第一周：机器学习基础与单变量线性回归

- 机器学习的定义与主要类型
- 监督学习中的回归与分类
- 非监督学习中的聚类、异常检测与降维
- 单变量线性回归模型 $f_{w,b}(x)=wx+b$
- 均方误差代价函数 $J(w,b)$
- $J(w,b)$ 的二维梯度与批量梯度下降
- 参数同时更新与顺序更新的区别

### 第二周：多变量线性回归

- 多维特征、特征矩阵与向量化计算
- 多变量线性回归的代价函数与批量梯度下降
- Mean normalization 与 Z-score normalization
- 使用学习曲线检查收敛并选择学习率
- 特征工程、组合特征与多项式回归
- 多项式特征缩放、模型复杂度与外推风险

### 第三周：逻辑回归与正则化

- 二元分类、Sigmoid 函数与概率解释
- 线性及非线性判定边界
- 二元交叉熵代价函数与逻辑回归梯度下降
- 高级优化算法与一对多分类
- 欠拟合、过拟合与泛化能力
- 正则化线性回归和正则化逻辑回归
- 正则化参数 $\lambda$ 的作用与常见错误

## 仓库结构

```text
.
|-- thefirstweek.tex              # 第一周笔记源码
|-- thesecondweek.tex             # 第二周笔记源码
|-- thethirdweek.tex              # 第三周笔记源码
|-- output/
|   `-- pdf/
|       |-- thefirstweek.pdf      # 第一周可直接阅读的 PDF
|       |-- thesecondweek.pdf     # 第二周可直接阅读的 PDF
|       `-- thethirdweek.pdf      # 第三周可直接阅读的 PDF
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
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build thesecondweek.tex
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build thethirdweek.tex
```

编译结果位于 `build/`。提交内容前，可将最新 PDF 更新到公开文档目录：

```powershell
Copy-Item build/thefirstweek.pdf output/pdf/thefirstweek.pdf
Copy-Item build/thesecondweek.pdf output/pdf/thesecondweek.pdf
Copy-Item build/thethirdweek.pdf output/pdf/thethirdweek.pdf
```

使用 VS Code 时，安装 LaTeX Workshop 扩展后打开 `.tex` 文件即可按仓库配置自动编译。

## 提交到远程仓库

编译并确认 PDF 可以正常打开后，可在仓库根目录执行：

```powershell
git status
git add README.md thethirdweek.tex output/pdf/thethirdweek.pdf
git commit -m "Add week 3 logistic regression notes"
git push origin main
```

提交前建议先用 `git status` 检查文件列表。`build/`、LaTeX 中间文件和本地临时文件已经由 `.gitignore` 排除，不需要手工加入版本控制。

## 许可证与说明

本仓库中原创的笔记源码与排版代码采用 [MIT License](LICENSE) 发布。课程名称、课程内容以及可能引用的第三方材料，其权利仍归各自权利人所有。
