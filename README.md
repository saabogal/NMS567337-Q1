![Q_banner](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/banner.png)

## ![qlogo](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/qloqo.png) **Quiz Twelve**

```yaml

Name of QuantLet : NMMS6

Published in : Null

Description : 'Quiz 6 Numerical Methods of Mathematical Statistics; Prove Theorem 28 and 29' 

Keywords : 'Weak Law of Large Numbers, Convergence Theory, Convergence properties'

Author : Luis Alejandro Sarmiento Abogado

Submitted : Tue, December 02 2015 by Luis Alejandro Sarmiento Abogado

Datafile : Null

```
[Quiz twelve.pdf](https://github.com/saabogal/NMS567337-Q1/files/50959/Quiz.eleven.pdf)

```tex

%% LyX 2.1.4 created this file.  For more info, see http://www.lyx.org/.
%% Do not edit unless you really know what you are doing.
\documentclass[english]{article}
\usepackage[T1]{fontenc}
\usepackage[utf8]{luainputenc}
\usepackage{color}
\usepackage{amsmath}
\usepackage{stackrel}
\usepackage{esint}
\usepackage{babel}
\begin{document}

\title{\textcolor{blue}{\large{}Numerical Methods of Mathematical Statistics }}

\maketitle

\section{Quiz 11 (8-3)}

Prove theorem 28 and 29\\
Theorem 28: let $\left\{ X_{i}\right\} $ be iid with cdf F, the existence
of constants $a_{n}$ for which $n^{-1}\sum_{i=1}^{n}X_{i}-a_{n}\overset{p}{\rightarrow0}$
\begin{itemize}
\item if $\left\{ x_{i}\right\} _{i=1}^{n}$ is iid with a given cdf F by
theorem 27 we get that $n^{-1}\stackrel[i=1]{n}{\sum}x_{i}\rightarrow\mu=E(x)$
and thus we can start working with theorem 28 that states $n^{-1}\stackrel[i=1]{n}{\sum}x_{i}-a_{n}\rightarrow0$
.
\item Given that every comulative distribution F is non decreasing and right
continuous, and furthermore, if F is abosultelly continuous we get
that $F(n)-F(-n)=P(-n<x\leq b)=\int_{a}^{b}f(x)dx$ = 1 
\item Finally we need to conclude in order to be consistent with the weak
law of large numbers that $a_{n}=E(x)=\int_{-n}^{n}xf(x)dx=\int_{-n}^{n}xdF(x)$.
Thus confirming that theorem 28 is consistent.
\end{itemize}
Theorem 29: Let $X,X_{1},X_{2}.....$ be iid and $\overline{X}_{n}=n^{-1}\sum_{i=1}^{n}X_{i}$.
Then if $E\mid X\mid^{2}<\infty$, then $\overline{X_{n}}\overset{2nd}{\longrightarrow}\mu=EX$:
\begin{itemize}
\item We start by stating $y_{i}=(x_{n}-\mu)$ which due to continuity is
a iid; furthermore is easy to conclude that $E(y_{i})\longrightarrow0$
and thus $E(\mid x_{n}-\mu\mid^{2})=n^{-2}\sum_{i=1}^{n}Var(y_{i})=n^{-2}n\sigma^{2}=n^{-1}\sigma^{2}\longrightarrow0$
giving enough prove for theorem 29
\end{itemize}
Alternative form:
\begin{itemize}
\item We proceed to prove the theorem by stating that $X{}_{i}\sim N(\mu,\sigma^{2})$. 
\item Variance is given by $S^{2}=n^{-1}\sum_{i=1}^{n}(X_{i}-\overline{X}_{n})^{2}$,
$E(\overline{X}_{n})=\mu,$ $Var(\overline{X}_{n})=\frac{\sigma^{2}}{n}$,
$E(S_{n}^{2})=\sigma^{2}$
\item We now proceed to prove the theorem through the moment generating
function. $M_{\overline{X}_{n}}(t)=E(e^{t\overline{X_{n}}})=E(e^{\frac{t}{n}\sum_{i=1}^{n}X_{i}})=Exp\left\{ 1+\mu t+\frac{t^{2}\frac{\sigma^{2}}{n}}{2}\right\} $
= $exp\left\{ \mu t+\frac{t^{2}\frac{\sigma^{2}}{n}}{2}\right\} $
Which is the moment generating function of $\overline{X}_{n}\sim N(\mu,\frac{\sigma^{2}}{n})$
and thus $\underset{n\rightarrow\infty}{lim}mgf(\overline{X}_{n})=\mu t$
confirming that $\overline{X_{n}}\overset{2nd}{\longrightarrow}\mu=EX$\end{itemize}

\end{document}

```

