# latexbookdemo
A book demo


```latex

\documentclass[10pt,letter,space]{book}

\usepackage[utf8]{inputenc}
\usepackage{amsmath}
\usepackage{amsfonts}
\usepackage{amssymb}
\usepackage{graphicx}
\usepackage{layout}
\usepackage{lipsum}
\usepackage{zhlipsum}
\usepackage{ctex}
\usepackage{lastpage} % 计算总的页面数
\usepackage{emptypage}% 清除空白页的页眉

%----------全局设置页眉和页脚的方法---------------
\usepackage{fancyhdr}
\pagestyle{fancy}

%设置页眉（E: L,C,R    ||   O:L,C,R）
\fancyhf{}  % 清除之前设置的fancy的版式


%\fancyhead[ER]{\leftmark} %设置左页右侧内容，章标题中的英文字母默认为大写形式
\fancyhead[ER]{\nouppercase{\leftmark}} %  设置左页右侧内容,修改章标题中的英文为小写形式
\fancyhead[OL]{\rightmark}%设置右页左侧内容


%\fancyhead[EC]{\nouppercase{\leftmark}} %  设置左页面中间显示的内容
%\fancyhead[OC]{\rightmark}%设置右页左侧内容
\renewcommand{\headrulewidth}{0.4pt} %设置页眉线的宽度

%设置页眉线
\fancyhead[EL]{\thepage}%设置左页左侧显示当前页码
\fancyhead[OR]{\thepage}%设置右页右侧显示当前页码
\renewcommand{\footrulewidth}{0pt} %设置页脚线的宽度



%设置页脚
%\fancyfoot[C]{第 \thepage / \pageref{LastPage}页}
%\renewcommand{\footrulewidth}{0pt}

%\pagestyle{headings}% 系统默认设置的版式，也是四大版式之一，其他的还有empty，plain和myheading


%------清除各章节首页标题的页眉和页脚，页码等内容[重要]---
\fancypagestyle{plain}{\fancyhf{}\renewcommand{\headrulewidth}{0pt}}


\title{\vspace{-30mm}\heiti \Huge 计算智能\\Intelligent Computing\thanks{注：国际通用的翻译方式}}
\author{张庆科 }
\date{\today}

\begin{document}
	\maketitle	
	\tableofcontents
	\frontmatter  % 前文区设置
	
	
%   ---------------------------------------------------------

   \mainmatter   %以下为主文区设置
%   ---------------------------------------------------------

\part{上篇}
	\chapter{绪论}
%	\pagenumbering{Roman}
The following part can be regarded as an illustration of 计算智能 namely， intelligence computation。
	\section{计算智能概念}
    \lipsum[1-4]
	\section{计算智能原理}
	  \lipsum[5-9]
%系统默认消除空白页和页眉的命令
%\clearpage{\pagestyle{empty}\cleardoublepage}
%\cleardoublepage
%   ---------------------------------------------------------
\chapter{智能计算数学基础 }
%\pagenumbering{arabic}
	\section{基本运算}
	\lipsum[10-16]
	\section{高等数学}
	\lipsum[5-9]
	
	\section{线性代数}
	\lipsum[25-30]

	\section{概率统计}
	\lipsum[35-40]
	
	\section{统计学习}
	\lipsum[55-60]
	\lipsum[25-30]
	
\clearpage{\pagestyle{fancy}\cleardoublepage}

%   ---------------------------------------------------------

\chapter{计算智能和机器学习}
%\pagenumbering{arabic}
\section{机器学习}
\lipsum[10-16]
\section{监督学习}
\lipsum[5-9]

\section{非监督学习}
\lipsum[25-30]
中文显示， 能正常的显示任何的字符了
\clearpage{\pagestyle{empty}\cleardoublepage}



\part{下篇}
\chapter{进化计算}
%\pagenumbering{arabic}
\section{差分进化算法}
\lipsum[10-12]
\section{粒子群优化算法}
\lipsum[5-7]
\chapter{神经网络}
\section{神经网络概念}
\lipsum[11-12]
\section{神经网络发展}
\lipsum[12-14]
\section{感知机算法}
\lipsum[15-16]
\section{神经网络}
\lipsum[16-17]
\section{卷积神经网络}
\lipsum[17-18]
\chapter{模糊系统}
\section{模糊系统概念}
\lipsum[19-20]
\section{模糊系统原理}
\lipsum[20-21]


%-----------------------------
\backmatter  % 后文区

\end{document}

```


