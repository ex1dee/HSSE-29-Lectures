>**Алгебраическая поверхность**
>$A_{1}x^{\alpha_{1}} y^{\beta_{1}}z^{\gamma_{1}}+A_{2}x^{\alpha_{2}}y^{\beta_{2}}z^{\gamma_{2}} + \dots + A_{n}x^{\alpha_{n}}y^{\beta_{n}}z^{\gamma_{n}} = 0, \ \alpha_{i}, \beta_{i}, \gamma_{i}$ - целые неотрицательные $max_{i=1,..,n}(\alpha_{i} + \beta_{i} + \gamma_{i}) = m$ - порядок поверхности

$x = 0, x^2 = 0, x^{20} = 0$ - разные поверхности

>**Алгебраическая линия на плоскости**
>$A_{1}x^{\alpha_{1}} y^{\beta_{1}}+A_{2}x^{\alpha_{2}}y^{\beta_{2}} + \dots + A_{n}x^{\alpha_{n}}y^{\beta_{n}}=0, \alpha_{i}, \beta_{i}$ - целые неотрицательные
>$max_{i=1,..,n}(\alpha_{i} + \beta_{i}) = m$ - порядок линии

>При изменении системы координат порядок алгебраической линии/поверхности не меняется

*Доказательство*
$O(\bar{e}_{1}, \bar{e}_{2}), O'(\bar{e}'_{1}, \bar{e}'_{2})$
$A_{1}x^{\alpha_{1}} y^{\beta_{1}}+A_{2}x^{\alpha_{2}}y^{\beta_{2}} + \dots + A_{n}x^{\alpha_{n}}y^{\beta_{n}}=0$ – уравнение порядка $p$

$$
\begin{cases}
x = a_{1}x' + b_{1}y' + c_{1} \\
y = a_{2}x' + b_{2}x' +c_{2}
\end{cases}
$$
$(a_{1}x+b_{1}y'+c_{1})^\alpha(a_{2}x+b_{2}y+c_{2})^\beta$
$\ \forall x^{\alpha'}y^{\beta'} \to \alpha' + \beta' \leq \alpha + \beta$

$p\to p', p' \leq p$, т.е. при переходе порядок не увеличивается
$p'\to p, p\leq p'$, т.е. при обратном переходе порядок не увеличивается
$\implies p=p'$

>Сколько общих точек может иметь поверхность $n-го$ порядка и прямая?
>Ответ: $0, 1, \dots, n$ или $\infty$, если прямая целиком лежит на поверхности

*Доказательство*
$$
l:\begin{cases}
x=x_{0}+a_{1}t \\
y=y_{0}+a_{2}t \\
z=z_{0}+a_{3}t
\end{cases}
$$

После подстановки в уравнение поверхности получим многочлен степени $\leq n \implies$ вещественных корней $\leq n$; либо тождество $0=0$. Тогда все точки прямой лежат на поверхности

>Линия 2 порядка на плоскости (будем рассматривать в ПДСК):
>$Ax^2+2Bxy+Cy^2+2Dx+2Ey+F=0, \ A^2 + B^2 + C^2 > 0$

___

$$
\Delta = \begin{vmatrix}
A & B  \\
B & C
\end{vmatrix}
$$

>Можно выбрать ПДСК, в которой линия 2 порядка будет иметь один из 9 канонических видов:

Линии элиптического типа $\Delta>0$:
1. $\frac{x^2}{a}+\frac{y^2}{b}=1, a\geq b>0$ - эллипс
2. $\frac{x^2}{a}+\frac{y^2}{b}=-1;  a, b \neq 0$ - мнимый эллипс
3. $\frac{x^2}{a}+\frac{y^2}{b}=0; a, b \neq 0$ - пара мнимых пересекающихся прямых

Линии гиперболического типа $\Delta < 0:$
4. $\frac{x^2}{a^2} - \frac{y^2}{b^2} = 1; a, b > 0$ 
5. $\frac{x^2}{a^2}-\frac{y^2}{b^2}=0; a, b > 0$ 

Линии параболического типа $\Delta=0:$
6. $y^2=2px; p>0$
7. $y^2=a^2; a \neq 0$
8. $y^2=-a^2; a \neq 0$
9. $y^2=0; a \neq 0$

>**Теорема**
>Для любой линии 2 порядка можно найти такую систему координат, что её уравнение можно привести к одному из 9 канонических видов

*Доказательство*
1
к $B \geq 0, A \geq C$
($x', y'$)

Пусть $B > 0$. Покажем, что найдётся такой угол поворота, что $B = 0 $
$x = x'\cos \alpha - y'\sin \alpha$
$y = y'\sin\alpha + y'\cos\alpha$

$A' = A\cos^2\alpha + 2B\cos\alpha \sin\alpha + C\sin^2\alpha$
$2B' = A(-2\sin\alpha \cos\alpha) + 2B(\cos^2\alpha-\sin^2\alpha) + C(2\sin\alpha \cos\alpha)$
$C' = A\sin^2\alpha - 2B\sin\alpha \cos\alpha+C\cos^2\alpha$

$$
\Delta=\begin{vmatrix}
A & B \\
B & C
\end{vmatrix} = \begin{vmatrix}
A' & B' \\
B' & C'
\end{vmatrix}
$$

$A' + C' = A + C$
$2B\cos 2\alpha - A\sin \alpha = 0$
$A = C \implies \alpha = \frac{\pi}{4}$
$A\neq C = > tg 2\alpha = \frac{2B}{A - C}$

2
$Ax^2+Cy^2+2Dx+2Ey+F = 0$
$\Delta > 0 \implies AC > 0, A, C \neq 0$
$\Delta < 0 \implies AC < 0, A,C \neq 0$

$ax^2+2bx=a\left( x^2+\frac{2b}{a}x + \left( \frac{b}{a} \right)^2 - \left( \frac{b}{a} \right)^2 \right) = a\left( x+\frac{b}{a} \right)^2 - \frac{b^2}{a}$
$x + \frac{b}{a} = x'$
$A'(x')^2+B(y')^2=m$
$A'(x')^2 = \frac{(x')^2}{sgn A'\left( \frac{1}{|A'|} \right)^2}$

$\Delta = 0$