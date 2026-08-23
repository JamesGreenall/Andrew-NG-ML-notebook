# 吴恩达机器学习笔记

这是一份使用 LaTeX 编写的中文机器学习学习笔记。目前内容涵盖机器学习基础、监督学习与非监督学习、线性回归、逻辑回归、神经网络、支持向量机、聚类、降维、异常检测、推荐系统和大规模机器学习。

本仓库是个人学习记录，并非吴恩达课程或相关平台的官方资料。

## 在线阅读

- [第一周笔记 PDF](output/pdf/thefirstweek.pdf)
- [第一周 LaTeX 源码](thefirstweek.tex)
- [第二周笔记 PDF](output/pdf/thesecondweek.pdf)
- [第二周 LaTeX 源码](thesecondweek.tex)
- [第三周笔记 PDF](output/pdf/thethirdweek.pdf)
- [第三周 LaTeX 源码](thethirdweek.tex)
- [第四周笔记 PDF](output/pdf/thefourthweek.pdf)
- [第四周 LaTeX 源码](thefourthweek.tex)
- [第五周笔记 PDF](output/pdf/thefifthweek.pdf)
- [第五周 LaTeX 源码](thefifthweek.tex)
- [第六周笔记 PDF](output/pdf/thesixthweek.pdf)
- [第六周 LaTeX 源码](thesixthweek.tex)
- [第七周笔记 PDF](output/pdf/theseventhweek.pdf)
- [第七周 LaTeX 源码](theseventhweek.tex)
- [第八周笔记 PDF](output/pdf/theeighthweek.pdf)
- [第八周 LaTeX 源码](theeighthweek.tex)
- [第九周笔记 PDF](output/pdf/theninthweek.pdf)
- [第九周 LaTeX 源码](theninthweek.tex)
- [第十周笔记 PDF](output/pdf/thetenthweek.pdf)
- [第十周 LaTeX 源码](thetenthweek.tex)

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

### 第四周：神经网络的表述

- 高维多项式特征的数量爆炸与神经网络的使用动机
- 神经元、输入层、隐藏层、输出层与偏置单元
- 权重矩阵的记号、尺寸和层间连接
- 前向传播与矩阵化计算
- 神经网络自动学习高级特征的直观理解
- 用神经元表示 AND、OR、NOT 与 XNOR
- 多类分类的输出层和 one-hot 标签

### 第五周：神经网络的学习

- 神经网络代价函数与正则化
- 反向传播和误差项
- 参数展开、梯度检验和随机初始化
- 从前向传播到完整训练流程
- 自主驾驶等模块化应用

### 第六周：应用机器学习的建议与系统设计

- 训练集、交叉验证集和测试集
- 模型选择、偏差方差和学习曲线
- 误差分析与下一步决策
- 类别不平衡、查准率、查全率和 $F_1$
- 数据质量、数据分布和系统设计

### 第七周：支持向量机

- SVM 优化目标与折线损失
- 大间隔分类和支持向量
- 线性核、高斯核与非线性边界
- 参数 $C$、$\sigma$ 和模型选型

### 第八周：聚类与降维

- 无监督学习与 K-均值算法
- K-均值目标函数、随机初始化和簇数选择
- PCA 的数据压缩与可视化动机
- 协方差矩阵、主成分和投影
- 选择主成分数量、重建误差与使用建议

### 第九周：异常检测与推荐系统

- 高斯分布、异常概率和阈值 $\varepsilon$
- 异常检测系统的开发与评价
- 异常检测和监督学习的适用场景
- 协同过滤、用户参数和物品特征
- 低秩矩阵分解、向量化和均值归一化

### 第十周：大规模机器学习与图片文字识别

- 随机梯度下降、小批量梯度下降和收敛
- 在线学习、MapReduce 和数据并行
- 图片文字识别的端到端流程
- 滑动窗口、数据收集和上限分析

## 仓库结构

```text
.
|-- thefirstweek.tex              # 第一周笔记源码
|-- thesecondweek.tex             # 第二周笔记源码
|-- thethirdweek.tex              # 第三周笔记源码
|-- thefourthweek.tex             # 第四周笔记源码
|-- thefifthweek.tex              # 第五周笔记源码
|-- thesixthweek.tex              # 第六周笔记源码
|-- theseventhweek.tex            # 第七周笔记源码
|-- theeighthweek.tex             # 第八周笔记源码
|-- theninthweek.tex              # 第九周笔记源码
|-- thetenthweek.tex              # 第十周笔记源码
|-- output/
|   `-- pdf/
|       |-- thefirstweek.pdf      # 第一周可直接阅读的 PDF
|       |-- thesecondweek.pdf     # 第二周可直接阅读的 PDF
|       |-- thethirdweek.pdf      # 第三周可直接阅读的 PDF
|       |-- thefourthweek.pdf     # 第四周可直接阅读的 PDF
|       |-- thefifthweek.pdf      # 第五周可直接阅读的 PDF
|       |-- thesixthweek.pdf      # 第六周可直接阅读的 PDF
|       |-- theseventhweek.pdf    # 第七周可直接阅读的 PDF
|       |-- theeighthweek.pdf     # 第八周可直接阅读的 PDF
|       |-- theninthweek.pdf      # 第九周可直接阅读的 PDF
|       `-- thetenthweek.pdf      # 第十周可直接阅读的 PDF
|-- templates/
|   |-- notebook-template.tex     # 笔记排版模板示例
|   `-- weekly-note-style.tex     # 第五至第十周共用排版样式
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
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build thefourthweek.tex
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build thefifthweek.tex
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build thesixthweek.tex
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build theseventhweek.tex
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build theeighthweek.tex
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build theninthweek.tex
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=build thetenthweek.tex
```

编译结果位于 `build/`。提交内容前，可将最新 PDF 更新到公开文档目录：

```powershell
Copy-Item build/thefirstweek.pdf output/pdf/thefirstweek.pdf
Copy-Item build/thesecondweek.pdf output/pdf/thesecondweek.pdf
Copy-Item build/thethirdweek.pdf output/pdf/thethirdweek.pdf
Copy-Item build/thefourthweek.pdf output/pdf/thefourthweek.pdf
Copy-Item build/thefifthweek.pdf output/pdf/thefifthweek.pdf
Copy-Item build/thesixthweek.pdf output/pdf/thesixthweek.pdf
Copy-Item build/theseventhweek.pdf output/pdf/theseventhweek.pdf
Copy-Item build/theeighthweek.pdf output/pdf/theeighthweek.pdf
Copy-Item build/theninthweek.pdf output/pdf/theninthweek.pdf
Copy-Item build/thetenthweek.pdf output/pdf/thetenthweek.pdf
```

使用 VS Code 时，安装 LaTeX Workshop 扩展后打开 `.tex` 文件即可按仓库配置自动编译。

## 提交到远程仓库

编译并确认 PDF 可以正常打开后，可在仓库根目录执行：

```powershell
git status
git add README.md templates/weekly-note-style.tex thefourthweek.tex thefifthweek.tex thesixthweek.tex theseventhweek.tex theeighthweek.tex theninthweek.tex thetenthweek.tex output/pdf/thefourthweek.pdf output/pdf/thefifthweek.pdf output/pdf/thesixthweek.pdf output/pdf/theseventhweek.pdf output/pdf/theeighthweek.pdf output/pdf/theninthweek.pdf output/pdf/thetenthweek.pdf
git commit -m "Add weeks 5 to 10 machine learning notes"
git push origin main
```

提交前建议先用 `git status` 检查文件列表。`build/`、LaTeX 中间文件和本地临时文件已经由 `.gitignore` 排除，不需要手工加入版本控制。

## 许可证与说明

本仓库中原创的笔记源码与排版代码采用 [MIT License](LICENSE) 发布。课程名称、课程内容以及可能引用的第三方材料，其权利仍归各自权利人所有。
