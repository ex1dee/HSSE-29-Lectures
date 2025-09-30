>**Смешанное произведение**
>В упорядоченной тройке $\bar{a}, \bar{b}, \bar{c}$
>$(\bar{a}, \bar{b}, \bar{c}) = ([\bar{a}, \bar{b}], \bar{c})$

>$(\bar{a}, \bar{b}, \bar{c})$ = $V_{\pm}$ параллелепипеда, построенного на $\bar{a}, \bar{b}, \bar{c}$
>$\bar{a}, \bar{b}, \bar{c}$ - компланарны $\implies V_{\pm} = 0$
>$\bar{a}, \bar{b}, \bar{c}$ - некомпланарны $\implies$ $+V$, если правая тройка; $-V$, если левая

>$\bar{a}, \bar{b}$ - коллинеарны - верно, $0=0$
>$\bar{a}, \bar{b}$ - неколлинеарны - $([\bar{a}, \bar{b}], \bar{c}) = |[\bar{a}, \bar{b}]| * Пр_{[\bar{a}, \bar{b}]}\bar{c}$,
>где $|[\bar{a}, \bar{b}]| = S_{параллелограмма}$, $|Пр_{[\bar{a}, \bar{b}]} \bar{c}| = h_{параллелепипеда} \implies ([\bar{a}, \bar{b}], \bar{c}) = V_{параллелепипеда}$

>$\bar{a}, \bar{b}, \bar{c}$ - некомпланарная правая тройка векторов 
>$(\bar{a}, \bar{b}, \bar{c}) = (\bar{b}, \bar{c}, \bar{a}) = (\bar{c}, \bar{a}, \bar{b}) = -(\bar{a}, \bar{c}, \bar{b}) = -(\bar{b}, \bar{a}, \bar{c}) = -(\bar{c}, \bar{b}, \bar{a})$
>$([\bar{a}, \bar{b}], \bar{c}) = (\bar{a}, \bar{b}, \bar{c}) = (\bar{b}, \bar{c}, \bar{a}) = ([\bar{b}, \bar{c}], \bar{a})$

>$(\bar{a}_{1} + \bar{a}_{2}, \bar{b}, \bar{c}) = (\bar{a_{1}}, \bar{b}, \bar{c}) + (\bar{a}_{2}, \bar{b}, \bar{c})$
>$(\alpha \bar{a}, \bar{b}, \bar{c}) = \alpha(\bar{a}, \bar{b}, \bar{c})$
>$(\alpha \bar{a}_{1} + \alpha_{2} \bar{a}_{2}, \bar{b}, \bar{c}) = \alpha_{1}(\bar{a}_{1}, \bar{b}, \bar{c}) + \alpha_{2}(\bar{a_{2}}, \bar{b}, \bar{c})$

>$\ \forall \bar{a}, \bar{b}_{1}, \bar{b}_{2}, \bar{c},\ \forall \beta_{1}\in \mathbb{R}, \beta_{2} \in \mathbb{R}$
>$[\beta_{1}\bar{b}_{1} + \beta_{2}\bar{b}_{2}, \bar{c}] = \beta_{1}[\bar{b}, \bar{c}] + \beta_{2}[\bar{b}_{2}, \bar{c}]$

$(\bar{a}, [\beta_{1}\bar{b}_{1} + \beta_{2}\bar{b}_{2}], \bar{c}) = \beta_{1}(\bar{a}, [\bar{b}_{1}, \bar{c}]) + \beta_{2}(\bar{a}, [\bar{b}_{2}, \bar{c}])$
$(\bar{a}, [\beta_{1}\bar{b}_{1} + \beta_{2}\bar{b}_{2}], \bar{c}) = (\bar{a}, \beta_{1}[\bar{b}_{1}, \bar{c}]) + (\bar{a}, \beta_{2}[\bar{b}_{2}, \bar{c}])$ (\*))

Подставим вместо $\bar{a}$ последовательно $\bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3} (ОНБ)$
$\bar{a} = \bar{e}_{1} \implies (*)$ - первая координата $[\beta_{1}\bar{b}_{1} + \beta_{2}\bar{b}_{2}, \bar{c}] = \beta_{1}[\bar{b}_{1}, \bar{c}] + \beta_{2}[\bar{b}_{2}, \bar{c}]$ (линейная комбинация первых векторов)


> $[\bar{a}, \bar{b}], [\bar{b}, \bar{c}], [\bar{c}, \bar{a}]$ - ЛНЗ $\iff \bar{a}, \bar{b}, \bar{c}$ - ЛНЗ

1. $\bar{a}, \bar{b}, \bar{c}$ - компланарные
Тогда $[\bar{a}, \bar{b}], [\bar{b}, \bar{c}], [\bar{c}, \bar{a}]$ коллинеарны
2. $\bar{a}, \bar{b}, \bar{c}$ - некомпланарные
Рассмотрим $\alpha_{1}[\bar{a}, \bar{b}] + \alpha_{2}[\bar{b}, \bar{c}] + \alpha_{3} [\bar{c}, \bar{a}] = 0$. Умножим скалярно на $\bar{c}$.
$\alpha_{1}(\bar{a}, \bar{b}, \bar{c}) + \alpha_{2}*0 + \alpha_{3}*0 = 0 \implies \text{т.к. } (\bar{a}, \bar{b}, \bar{c}) \neq 0 \text{, то } \alpha_{1} = 0$. 
Аналогично $\alpha_{2}=\alpha_{3}=0 \implies (\bar{a}, \bar{b}, \bar{c}) - ЛНЗ$

>$\bar{e}_{1}' = \frac{[\bar{e}_{2}, \bar{e}_{3}]}{(\bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3})}, \bar{e}_{2}' = \frac{[\bar{e}_{3}, \bar{e}_{3}]}{(\bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3})}, \bar{e}_{3}' = \frac{[\bar{e}_{1}, \bar{e}_{2}]}{(\bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3})}$ - биортогональный базис к базису $\bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3}$

>$\bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3}$ - базис
>$\bar{a} = (a_{1}, a_{2}, a_{3}), \bar{b} = (b_{1}, b_{2}, b_{3}), \bar{c} = (c_{1}, c_{2}, c_{3})$ - его векторы
>
$$
\begin{array}{}
(\bar{a}, \bar{b}, \bar{c}) = (a_{1}\bar{e}_{1} + a_{2}\bar{e}_{2} + a_{3}\bar{e}_{3}, b_{1}\bar{e}_{1} + b_{2}\bar{e}_{2} + b_{3}\bar{e}_{3}, c_{1}\bar{e}_{1} + c_{2}\bar{e}_{2} + c_{3}\bar{e}_{3}) \\
\text{ всего 6 штук, где } \bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3} \text{ (с одинаковыми индексами)} \\
=(\bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3})(a_{1}b_{2}c_{3} + a_{2}b_{3}c_{1} - a_{2}b_{1}c_{3} - a_{3}b_{2}c_{1}) =  \\
=(\bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3}) \begin{vmatrix}
a_{1}&a_{2}&a_{3} \\
b_{1}&b_{2}&b_{3} \\
c_{1}&c_{2}&c_{3}
\end{vmatrix} = \begin{vmatrix}
a_{1}&a_{2}&a_{3} \\
b_{1}&b_{2}&b_{3} \\
c_{1}&c_{2}&c_{3}
\end{vmatrix} \text{ в правом ОНБ}
\end{array}
$$

$$
V = 0 \iff \bar{a}, \bar{b}, \bar{c} \text{ компланарны} \iff
\begin{vmatrix}
a_{1}&a_{2}&a_{3} \\
b_{1}&b_{2}&b_{3} \\
c_{1}&c_{2}&c_{3}
\end{vmatrix} = 0
$$
$$
\bar{a}, \bar{b} - \text{ коллинеарны } \iff [\bar{a}, \bar{b}] = 0 \iff
\begin{vmatrix}
a_{2} & a_{3} \\
b_{2} & b_{3}
\end{vmatrix} = \begin{vmatrix}
a_{1} & a_{3} \\
b_{1} & b_{3}
\end{vmatrix}
= \begin{vmatrix}
a_{1} & a_{2} \\
b_{1} & b_{2}
\end{vmatrix} = 0
$$

>$$
>S^2 = |[\bar{a}, \bar{b}]| = |\bar{a}|^2|\bar{b}|^2\sin^2\alpha = |\bar{a}|^2|\bar{b}|^2 (1-\cos^2\alpha)
=
$$

>$\bar{a}(a_{1}, a_{2}), \bar{b}(b_{1}, b_{2}) \text{ в базисе } \bar{e}_{1}, \bar{e}_{2} \ (\bar{a}, \bar{b} - неколлинеарны)$ 
>$|\bar{n}|=1, \bar{n} \perp \bar{a}, \bar{b}$

$$
\begin{array}{}
S_{\pm}(\bar{a}, \bar{b}) = V_{\pm}(\bar{a}, \bar{b}, \bar{n})
= \begin{vmatrix}
a_{1} & a_{2} & 0 \\
b_{1} & b_{2}&0 \\
0 & 0& 1
\end{vmatrix}*(\bar{e}_{1}, \bar{e}_{2}, \bar{n})
= 
\begin{vmatrix}
a_{1}&a_{2} \\
b_{1}&b_{2}
\end{vmatrix} * S_{\pm}(\bar{e}_{1}, \bar{e}_{2}) = S_{\pm}(\bar{a}, \bar{b}) \\
\text{В правом ОНБ } S_{\pm}(\bar{a}, \bar{b}) = 
\begin{vmatrix}
a_{1}&a_{2} \\
b_{1}&b_{2}
\end{vmatrix} = a_{1}b_{2}-b_{1}b_{2} \implies S(\bar{a}, \bar{b}) = |a_{1}b_{2}-b_{1}a_{2}|
\end{array}
$$

>$[\bar{a}, [\bar{b}, \bar{c}]] = \bar{b}(\bar{a}, \bar{c}) - \bar{c}(\bar{a}, \bar{b})$

*Доказательство*

Выберем правый ОНБ $\bar{e}_{1}, \bar{e}_{2}, \bar{e}_{3}; \bar{e} ||\bar{b}$
$\bar{b}, \bar{c}, \bar{e}_{2}$ - компланарны
$\bar{e}_{3}$ определяется однозначно

$$
\bar{b} =
\begin{pmatrix}
\beta \\
0 \\
0 \\
\end{pmatrix}
,
\bar{c}= \begin{pmatrix}
\lambda_{1} \\
\lambda_{2} \\
0
\end{pmatrix}
,
\bar{a}=\begin{pmatrix}
 \alpha_{1} \\
\alpha_{2} \\
\alpha_{3}
\end{pmatrix}
$$
$$
[\bar{b}, \bar{c}] =
\begin{vmatrix}
\bar{e}_{1} & \bar{e}_{2} & \bar{e}_{3} \\
\beta & 0 & 0 \\
\lambda_{1} & \lambda_{2} & 0
\end{vmatrix}
= \begin{pmatrix}
0 \\
0 \\
\beta\lambda_{2}
\end{pmatrix}
$$
$$
[\bar{a}, [\bar{b}, \bar{c}]] = 
\begin{vmatrix}
\bar{e}_{1} & \bar{e}_{2} & \bar{e}_{3} \\
\alpha_{1} & \alpha_{2} & \alpha_{3} \\
0 & 0 & \beta\lambda_{2}
\end{vmatrix}
=
\begin{pmatrix}
\alpha_{2}\beta\lambda_{2} \\
-\alpha_{1}\beta\lambda_{2} \\
0
\end{pmatrix}
$$