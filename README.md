![Q_banner](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/banner.png)

## ![qlogo](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/qloqo.png) **Quiz Four**

```yaml

Name of QuantLet : NMMS4

Published in : Null

Description : 'Quiz 6 Numerical Methods of Mathematical Statistics; Show the characteristic functions of several distributions' 

Keywords : 'Characteristic Function, pdf, '

Author : Luis Alejandro Sarmiento Abogado

Submitted : Tue, December 02 2015 by Luis Alejandro Sarmiento Abogado

Datafile : Null

```
[Quiz4.pdf](https://github.com/saabogal/NMS567337-Q1/files/49923/Quiz.4.pdf)

```tex

%% LyX 2.1.4 created this file.  For more info, see http://www.lyx.org/.
%% Do not edit unless you really know what you are doing.
\documentclass[english]{article}
\usepackage[T1]{fontenc}
\usepackage[utf8]{luainputenc}
\usepackage{color}
\usepackage{amsmath}

\makeatletter

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% LyX specific LaTeX commands.
%% Because html converters don't know tabularnewline
\providecommand{\tabularnewline}{\\}

\makeatother

\usepackage{babel}
\begin{document}

\title{\textcolor{blue}{\large{}Numerical Methods of Mathematical Statistics }}

\maketitle

\section{Quiz 4.0}

Show the characteristic function of several distributions\\


\begin{tabular}{|c|c|c|}
\hline 
Distribution & pdf & cf\tabularnewline
\hline 
\hline 
Normal & $f(x)\text{=\ensuremath{\frac{1}{\sqrt{2\pi}}e^{-x^{2}}}}$ & $e^{it\mu-\frac{1}{2}\sigma^{2}t^{2}}$\tabularnewline
\hline 
Multivariate Normal & $f(x_{n})=\frac{1}{\sqrt{(2\pi)^{k}\mid\Sigma}\mid}exp\left\{ \frac{-1}{2}(x-\mu)^{T}\Sigma^{-1}(x-\mu)\right\} $ & $e^{it^{T}\mu-\frac{1}{2}t^{T}\sum t}$\tabularnewline
\hline 
Binomial & $f(k;n,p)=pr(X=k)=\left(\begin{array}{c}
n\\
k
\end{array}\right)p^{k}(1-p)^{n-k}$ & $(1-p+pe^{it})^{n}$\tabularnewline
\hline 
Poisson & $f(k;\lambda)=pr(X=k)=\frac{\lambda^{k}e^{-\lambda}}{k!}$ & $e^{\lambda(e^{it}-1)}$\tabularnewline
\hline 
Chi-squared & $X^{2}=\frac{1}{2^{\frac{k}{2}}\varGamma\left(\begin{array}{c}
k\\
2
\end{array}\right)}x^{\frac{k}{2}}e^{\frac{-x}{2}}$ & $(1-2it)^{-k/2}$\tabularnewline
\hline 
Exponential & $\lambda e^{-\lambda x}$ & $(1-it\lambda^{-1})^{-1}$\tabularnewline
\hline 
\end{tabular}
\end{document}


```

