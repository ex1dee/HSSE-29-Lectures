Подставим в уравнение линии 2 порядка $Ax^2+2Bxy+Cy^2+2Dx +2Ey+F =0$:
$\begin{cases} x=x_{0}+\alpha t  \\ y=y_{0}+\beta t\end{cases}$

$A(x_{0}+\alpha t)^2+2B(x_{0}+\alpha t)(y_{0}+\beta t) + \dots = 0$
$Pt^2+2Qt+R=0$

$P=A\alpha^2+2B\alpha\beta+C\beta^2$ – зависит от $\alpha,\beta$ с точностью до множителя $\neq 0$
$Q=(Ax_{0}+By_{0} + D)\alpha+(Bx_{0}+Cy_{0}+E)\beta = (A\alpha+B\beta)x_{0}+(B\alpha+C\beta)y_{0}+D\alpha+E\beta$
$R=Ax^2+2Bxy+Cy^2+2Dx +2Ey+F$

>**Асимптотическое направление** — направление $(\alpha, \beta)$, определяющее $P = 0$

>**Теорема**
>$\Delta = \begin{vmatrix}A & B  \\ B & C\end{vmatrix}$
>
>$\Delta < 0 \implies$ 2 асимптотических направления
>$\Delta = 0 \implies$ 1 асимптотическое направление
>$\Delta > 0 \implies$ нет асимптотических направлений

*Доказательство:*
$A\alpha^2+2B\alpha\beta+C\beta^2 = 0$

1. Пусть $C\neq 0$. Поделим на $\alpha^2$: $A + 2B \cdot \frac{\beta}{a} + C \cdot \frac{\beta^2}{\alpha^2} = 0$
$\frac{D}{4} = B^2 - AC = -\Delta$
$\Delta < 0 \implies$ 2 решения
$\Delta > 0 \implies$ 0 решений
$\Delta = 0 \implies$ 1 решение

2. Пусть $C = 0$. Тогда $\Delta=-B^2$
Если $B = 0$, то $\Delta = 0$ и 1 решение ?
Если $B\neq 0$, то $\Delta <0$ и 2 решения

___

>**Хорда линии 2 порядка** — отрезок, концы которого лежат на линии, а остальные его точки – нет

Хорда образуется из пересечения линии 2 порядка с прямой неасимптотического направления

>Рассмотрим $(\alpha, \beta)$. Получим параллельные хорды.

$\begin{cases} x=x_{0}+\alpha t  \\ y=y_{0}+\beta t\end{cases}, (x_{0}, y_{0})$ – середина хорды

Множество середин таких хорд назовём 
$(x_{0}, y_{0}) \text{ удовлетворяет } Q = (A\alpha+B\beta)x_{0}+(B\alpha+C\beta)y_{0}+D\alpha+E\beta = 0$
Тогда множество середин хорд лежит на прямой. 
Назовём эту прямую **диаметром линии 2 порядка**, сопряженным направлению $(\alpha, \beta)$

Причём $\alpha$ и $\beta$ одновременно не равны нулю, т.к. иначе
$\begin{cases} A\alpha+B\beta=0 \\ B\alpha+C\beta=0 \end{cases}$ $\implies A\alpha^2+2B\alpha\beta+C\beta^2=0$?

___

Пусть $G(x, y) = Ax^2+2Bxy+Cy^2+2Dx +2Ey+F$.

>Точку $O(x_{0}, y_{0})$ назовём **центром линии 2 порядка**, если 
>$\ \forall \alpha,\beta \in \mathbb{R} \to G(x_{0}+\alpha, y_{0}+\beta)=G(x_{0}-\alpha, y_{0}-\beta)$

$G(x_{0}+\alpha,y_{0}+\beta) = A(x_{0}+\alpha)^2+2B(x_{0}+\alpha)(y_{0}+\beta)+\dots =$  $G(x_{0}-\alpha,y_{0}-\beta) = A(x_{0}-\alpha)^2+2B(x_{0}-\alpha)(y_{0}-\beta)+\dots$

$\alpha(Ax_{0}+By_{0}+D)+\beta(Bx_{0}+Cy_{0}+E)=0$

$\begin{cases} Ax_{0}+By_{0}+D = 0 \\ Bx_{0}+Cy_{0}+E=0\end{cases}$

>Кривая называется **центральной**, если у неё ровно 1 центр 
>(все линии элиптического и гиперболического типов)
>Нецентральные линии – линии параболического типа

>**Теорема**
>Пусть линия 2 порядка задаёт непустое множество на плоскости и имеет центр.
>Тогда точка $O$ – центр симметрии 

