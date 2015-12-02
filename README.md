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
[Intro.pdf](https://github.com/saabogal/NMS567337-Q1/files/49018/Quiz.six.pdf)

```tex

\documentclass[english]{article}
\usepackage[T1]{fontenc}
\usepackage[utf8]{luainputenc}
\usepackage{color}
\usepackage{babel}
\begin{document}

\title{\textcolor{blue}{\large{}Numerical Methods of Mathematical Statistics}}

\maketitle

\section{Quiz 6 (5-3)}

Prove (19) for k=1,2,3,4 for N(0,1)

If K-moment of X exist and $\varphi x(T)$ has k derivative at zero,
then $\varphi_{X}^{(k)}(T)\mid_{t=0}=i^{k}E(X^{k})$
\begin{itemize}
\item CF of a standard normal is $\varphi x(t)=exp\left\{ i\mu t+\frac{1}{2}\sigma^{2}t^{2}\right\} $ 
\item it follows that $\varphi^{'}x(t)=$ $(\sigma^{2}t+i\mu)e^{\frac{s^{2}t^{2}+2i\mu t}{2}}$
such that at t=0 gives us $i\mu$ = $i^{1}E(X^{1})$ 
\item $\varphi^{''}x(t)=(\sigma^{4}t^{2}+2i\mu\sigma^{2}t+\sigma^{2}-\mu^{2})e^{\frac{s^{2}t^{2}+2i\mu t}{2}}$
which evaluated at t=0 gives us $\sigma^{2}-\mu^{2}=i^{2}E(X^{2})$ 
\item $\varphi^{'''}x(t)=(\sigma^{2}t+i\mu)(\sigma^{4}t^{2}+2i\mu\sigma^{2}t+3\sigma^{2}-\mu^{2})e^{\frac{s^{2}t^{2}+2i\mu t}{2}}$
Which evaluated at t=0 gives us $i\mu(3\sigma^{2}-\mu^{2})=i^{3}E(X^{3})$
\item $\varphi^{''''}x(t)=(\sigma^{8}t^{4}+i\mu\sigma^{6}t^{3}+(6\sigma^{6}-6\mu^{2}\sigma^{4})t^{2}+(12i\mu\sigma^{4}t+4i\mu^{3}\sigma^{2})t+3\sigma^{4}-6\mu^{2}\sigma^{2}+\mu^{4})e^{\frac{s^{2}t^{2}+2i\mu t}{2}}$
Which evaluated at t=o gives us $3\sigma^{4}-6\mu^{2}\sigma^{2}+\mu^{4}=i^{4}E(X^{4})$
\end{itemize}
Thus proving the theorem for the first four moments 
\end{document}

```

