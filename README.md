# TJU-Paper-template
## 仓库说明

内容为天津大学论文模板,仅供个人使用.内容与geniusLcy大佬有较多相似部分,特别感谢大佬的帮助🙏

所参考仓库的地址:

https://github.com/twtstudio/TJUThesisLatexTemplate/tree/master/Thesis

https://github.com/geniusLcy/TJU-report-template

## 文件说明

+ Thesis 内为[TJU-report-template.zip]解压内容,是模板核心内容
+ reference 内有2个压缩包,分别是本仓库参考的两个仓库的压缩包

## 使用说明

+ 使用overleaf选择 新建项目 -> 上传项目 -> 选择[TJU-report-template.zip]即可. 之后在body.tex内进行修改
+ **注意** compiler需选择XeLatex

## 数学公式

数学公式的具体书写方式参考文档《[一份不太简短的 LaTeX 介绍](http://www.ctan.org/tex-archive/info/lshort/chinese/)》，注意：需要标号的公式请在`equation`环境下配合`\label{}`标签使用，在需要引用的地方使用`\eqref{}`命令引用相应公式。示例如下：

```latex
销售商决策如式~\eqref{rcond}~所示：
\begin{equation}
\label{rcond}
\left\{\begin{array}{l}
p_{1s}=v_h-(v_h-p_2)\mathbb{E}(\varphi) \\
p_{2s}=v_l \\
q_s \in \underset{q \geq 0}{\mathrm{argmax}} \beta_R (q, p_1, p_2) \\
\end{array}\right.
\end{equation}
```

## 插图与表格

参考文档与模板示例。建议图像使用`.eps`矢量格式，放入 `figures` 目录下。

插图示例：

```latex
图像如图~\ref{fig:simuP1P2Result}~所示。
\begin{figure}[htbp!]
\centering
\includegraphics[width=0.75\textwidth]{figures/p1p2figure.eps}
\caption{最优$p_1, p_2$仿真结果}\label{fig:simuP1P2Result}
\vspace{-1em}
\end{figure}
```

表格示例：

```latex
\begin{table}[htbp]
\caption{符合本科生毕业论文绘图规范的表格}\label{tab:table1}
\vspace{0.5em}\centering\wuhao
\begin{tabular}{ccccc}
\toprule[1.5pt]
$D$(in) & $P_u$(lbs) & $u_u$(in) & $\beta$ & $G_f$(psi.in)\\
\midrule[1pt]
 5 & 269.8 & 0.000674 & 1.79 & 0.04089\\
10 & 421.0 & 0.001035 & 3.59 & 0.04089\\
20 & 640.2 & 0.001565 & 7.18 & 0.04089\\
 5 & 269.8 & 0.000674 & 1.79 & 0.04089\\
10 & 421.0 & 0.001035 & 3.59 & 0.04089\\
20 & 640.2 & 0.001565 & 7.18 & 0.04089\\
 5 & 269.8 & 0.000674 & 1.79 & 0.04089\\
10 & 421.0 & 0.001035 & 3.59 & 0.04089\\
20 & 640.2 & 0.001565 & 7.18 & 0.04089\\
 5 & 269.8 & 0.000674 & 1.79 & 0.04089\\
10 & 421.0 & 0.001035 & 3.59 & 0.04089\\
20 & 640.2 & 0.001565 & 7.18 & 0.04089\\
\bottomrule[1.5pt]
\end{tabular}
\vspace{\baselineskip}
\end{table}
```

## 参考文献

所有参考文献在 `Thesis/references/reference.bib` 中。BibTex 格式的参考文献可通过以下步骤获得：

* 打开浏览器，访问 [Google Scholar](http://scholar.google.com)
* 查找你所需的文献
* 点击文献下方 引用/cite 按钮
* 在弹出框内点击 BibTex
* 复制新窗口里的文本粘贴到 reference.bib 中
* 在 body.tex 中需要引用的地方使用`\cite{}`命令进行引用，括号里填参考文献第一行左花括号后面的 identifier。如使用下面推荐的工具链可以实现参考文献自动补全

## 目录，字体，字号，编号，序号，页码，页眉，排版...

全都是自动的。
