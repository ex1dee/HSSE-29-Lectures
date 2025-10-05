>**Теорема Эйлера** 
>*Обобщение Малой теоремы Ферма*
>$a^{\phi(n)} \equiv_{n} 1$, если $НОД(a, n) = 1$

Рассмотрим остатки от деления на $n,$ взаимно простые с $n: r_{1}, r_{2}, \dots, r_{\phi(n)} (mod\ n)$
Умножим каждый остаток на $a: ar_{1}, ar_{2}, \dots, ar_{\phi(n)} (mod \ n)$. 
Все они взаимно просты с $n$ и не равны между собой
(иначе $ar_{i} \equiv_{n} ar_{j} \iff a(r_{i}-r_{j}) \equiv_{n} 0 \implies$ т.к. $a\not\equiv_{n}$ 0, то $r_{i} = r_{j}$)

Тогда $ar_{1}*ar_{2}*\dots*ar_{\phi(n)} \equiv_{n} r_{1}r_{2}\dots r_{\phi(n)}$. $НОД(r_{1}r_{2}\dots r_{\phi(n)}, n) = 1$, домножим на $r_{1}r_{2}\dots r_{\phi(n)}$
и получим $a^{\phi(n)} \equiv_{n} 1$

>**Алгоритм Евклида**
>$НОД(a, b) = НОД(b, a \% b)$

Начальные условия:
$a_{0} = a, a_{1} = b$
Промежуточные значения $gcd(a_{i-1}, a_{i}) = gcd(a_{i}, a_{i+1})$:
$a_{i-1}\%a_{i} = a_{i-1} - a_{i}\left\lfloor  \frac{a_{i-1}}{a_{i}}  \right\rfloor = a_{i+1}$
$a_{i-1} = a_{i}\left\lfloor  \frac{a_{i-1}}{a_{i}}  \right\rfloor + a_{i+1}, 0 \leq a_{i+1} < |a_{i}|$, $a_{i}$
Результат: 
$a_{t} = НОД(a_{0}, a_{1})$ - последний ненулевой остаток
$a_{t-1} = 0$

*Доказательство*
1. Докажем, что $НОД(a, b) = НОД(a - b, b)$.
Пусть $НОД(a, b) = d \ | \ a :d, b : d, d \to max$
$a :d, b : d \implies (a - b) : d$
Тогда $d$ - общий делитель $(a - b)$ и $b$.
Если $d$ - не наибольший общий делитель, то есть $\ \exists d' > d : НОД(a - b, b) = d'$
Тогда $(a - b) : d', b : d' \implies$ $a : d' \implies$ $d'$ - общий делитель $a$ и $b$, 
но т.к. $d' > d$, то $НОД(a, b) = d'$ - противоречие $\implies НОД(a - b, b) = d = НОД(a, b)$

2. Раз $НОД(a, b) = НОД(a - b, b)$, то $НОД(a, b) = НОД\left( a - \left\lfloor  \frac{a}{b}  \right\rfloor b, b \right) = НОД(a \% b, b)$

>**Расширенный алгоритм Евклида**
>Помимо $НОД(a, b)$ находит такие $x$ и $y$:
>$ax + by = d = НОД(a, b)$

Когда алгоритм Евклида закончился, мы получили:
$x_{t}\cdot0 + y_{t}*(НОД(a, b)) = НОД(a, b)$
Тогда для последнего шага возьмём начальные условия $x_{t} = 0, y_{t} = 1$

Пусть мы посчитали нужные коэффициенты $x_{i+1}$ и $y_{i+1}$, когда считали $НОД(b, a \% b)$:
$x_{i+1}b + y_{i+1}(a\%b) = d$
$x_{i+1}b + y_{i+1}\left( a - b \left\lfloor  \frac{a}{b}  \right\rfloor \right) = d$
$ay_{i+1} + b\left( x_{i+1} - \left\lfloor  \frac{a}{b}  \right\rfloor y_{i+1}\right) = d$
Тогда $(y_{i+1}, x_{i+1} - \left\lfloor  \frac{a}{b}  \right\rfloor y_{i+1})$ - решение для исходной пары, т.е.
$x_{i} = y_{i+1}$
$y_{i} = x_{i+1} - \left\lfloor  \frac{a}{b}  \right\rfloor y_{i+1}$

>**Решение диафантовых уровнений** 
>$ax + by = c$

$$

\begin{array}{} \\
\text{Пусть } d = НОД(a, b) \\
 \text{Если c} \not{:}\ \ d, \text{то решений нет}\\ \text{Если } c : d, \text{то }  \\
\begin{cases}
x = x_{0} + \frac{b}{d}t \\
y = y_{0}+\frac{b}{d}t
\end{cases} , t \in \mathbb{Z}
\end{array}
$$
*Доказательство*
Т.к. $a : d, b : d\implies ax+by:d$, то $c : d$

Рассмотрим два решения $ax + by = c$:
$ax_{1} + by_{1} = c$
$ax_{2} + by_{2} = c$

Их разность: $a(x_{1} - x_{2}) + b(y_{1} - y_{2}) = 0$
Пусть $a = da_{1}, b = db_{1}, НОД(a_{1}, b_{1}) = 1$ (иначе $НОД(a, b) > d$)
$da_{1}(x_{1} - x_{2}) + db_{1}(y_{1} - y_{2}) = 0 \iff a_{1}(x_{1} - x_{2}) + b_{1}(y_{1} - y_{2}) = 0$
$(x_{1}-x_{2}) : b \implies x_{1} - x_{2}=b_{1}t = \frac{b}{d}t, t \in \mathbb{Z}$
$(y_{1}-y_{2}) : a \implies y_{1} - y_{2}=a_{1}t = \frac{a}{d}t, t \in \mathbb{Z}$

Тогда, если $(x_{0}, y_{0})$ - частное решение $ax+by=c$, то
$x = x_{0}+\frac{b}{d}t, y= y_{0} + \frac{b}{d}t$

Как найти это частное решение:
Решим $ax' + by' = d$ расширенным алгоритмом Евклида
Умножим всё на $\frac{c}{d} \in \mathbb{Z}$: $a\left( \frac{c}{d}x' \right) + b\left( \frac{c}{d}x' \right) = c$
Т.е. $x_{0}=\frac{c}{d}x', y_{0} = \frac{c}{d}y'$

>Число $a$ является **квадратичным вычетом** (остатком) по модулю $n$, если 
>$\ \exists x\in \mathbb{Z}:x^2\equiv_{n}a$, $a \neq 0$ 
>иначе это **квадратичный невычет**

$V$ - множество квадратичных вычетов по модулю $n$
$N$ - множество квадратичных невычетов по модулю $n$

>$1^2, 2^2, \dots,\left( \frac{p-1}{2} \right)^2$ - все квадратичные вычеты по модулю $p$
>Количество квадратичных вычетов $=$ количество квадратичных невычетов $= \frac{p-1}{2}$

*Доказательство:*
Рассмотрим все квадратичные вычеты по модулю $p$:
$1^2, 2^2, \dots, (\frac{p-1}{2})^2, (\frac{p+1}{2})^2, \dots, (p-1)^2, p^2, \dots$

$(p+x)^2\equiv_{p}x^2 \implies$ Остатки $p^2, (p+1)^2, \dots$ просто
повторяют остатки $1^2, 2^2, \dots, (\frac{p-1}{2})^2, (\frac{p+1}{2})^2, \dots, (p-1)^2$

Также заметим, что $(p-x)^2\equiv_{p}x^2$ и
$1 \leq x \leq \frac{p-1}{2}$
$-\frac{p-1}{2} \leq -x \leq -1$
$\frac{p+1}{2} \leq p - x \leq p -1$
Следовательно, каждому остатку из $1^2, 2^2, \dots, \left( \frac{p-1}{2} \right)^2$
найдётся пара из $\left( \frac{p+1}{2} \right)^2, \dots, (p-1)^2$

Кроме того, $x_{i}^2 \not\equiv_{p} x_{j}^2$ при $x_{i} \neq x_{j}$
Иначе $(x_{i} - x_{j})(x_{i}+x_{j}) \equiv_{p} 0$. Тогда либо $x_{i} - x_{j} \equiv_{p} 0$, но это невозможно, т.к. $x_{i} \neq x_{j}$,
либо $x_{i}+x_{j} \equiv_{p}0$, но это также невозможно, т.к. $x_{i}+x_{j} < \frac{p-1}{2} * 2<p$ - противоречие.

Таким образом, все квадратичные вычеты по модулю $p$ - это числа $1^2, 2^2, \dots, \left( \frac{p-1}{2} \right)^2$.
Все ненулевые вычеты по модулю $p: 1, 2, \dots, p-1$.  Их $p-1$, из них $\frac{p-1}{2}$ квадратичных вычетов по модулю $p$ и $\left( p - \frac{p-1}{2}\right) = \frac{p-1}{2}$ квадратичных невычетов по модулю $p$.

>**Символ Лежандра** - $\left( \frac{a}{p} \right), a \in \mathbb{Z}, p > 2$ - простое ($\frac{a}{p}$ - не дробь!)
>$\left( \frac{a}{p} \right) = 0$, если $a : p$
>$\left( \frac{a}{p} \right) = 1$, если $a$ - квадратичный вычет по модулю p
>$\left( \frac{a}{p} \right) = -1$, если $a$ - квадратичный невычет по модулю p

> **Мультипликативность символа Лежандра**
> $\left( \frac{ab}{p} \right) = \left( \frac{a}{p} \right)*\left( \frac{b}{p} \right)$

*Доказательство:*

**1 случай**
Если $\left( \frac{a}{p} \right) = 0$ или $\left( \frac{b}{p} \right) = 0,$ то $\left( \frac{ab}{p} \right) = 0$ (*если $a : p$ или $b : p$*)
*Теперь рассмотрим случаи, когда $a  \not{:}\ \ p$ и $b  \not{:}\ \ p$.*

**2 случай**
Если $\left( \frac{a}{p} \right)=\left( \frac{b}{p} \right)=1$:
$a \equiv_{p} x^2, b \equiv_{p}y^2 \implies ab \equiv_{p}(xy)^2 \implies$ $\left( \frac{ab}{p} \right)=1$

**3 случай**
Теперь, без ограничения общности, предположим, что $\left( \frac{a}{p} \right) = 1, \left(\frac{b}{p}\right)=-1$
Очевидно, $\left( \frac{ab}{p} \right) \neq 0$. Предположим, что $\left( \frac{ab}{p} \right) = 1$.

Тогда $\ \exists x:a\equiv_{p}x^2, \ \exists y:ab\equiv_{p}y^2$
Т.к. $a \not\equiv_{p}0$, то $x\not\equiv_{p} 0 \implies НОД(x, p) = 1 \implies \ \exists x^{-1} : x\cdot x^{-1}\equiv_{p}1$
$\implies (x\cdot x^{-1})^2\equiv_{p}1 \iff x^2\cdot(x^{-1})^2\equiv_{p}1 \implies a\cdot(x^{-1})^2 \equiv_{p}1$
Домножим $ab\equiv_{p}y^2$ на $(x^{-1})^2$ и получим: $b\equiv_{p}y^2\cdot (x^{-1})^2 \implies \left( \frac{b}{p} \right)=1$ - противоречие.
Следовательно, если $\left( \frac{a}{p} \right)=1, \left( \frac{b}{p} \right)=-1$, то $\left( \frac{ab}{p} \right)=-1$

**4 случай**
Если $\left( \frac{a}{p} \right) = -1, \left( \frac{b}{p} \right)=-1$.
Рассмотрим ненулевые остатки при делении на $p: 1, 2, \dots, p - 1$
Умножим их на $c : НОД(c, p) = 1$, получим различные $c, 2c, \dots, (p-1)c$

Предположим, $c$ - невычет. 
Если $c$ умножить на каждые $\frac{p-1}{2}$ вычетов, то получим $\frac{p-1}{2}$ невычетов (*3 случай*)
Если $c$ умножить на каждые $\frac{p-1}{2}$ невычетов, то получим оставшиеся $p - \frac{p-1}{2} = \frac{p-1}{2}$ вычетов,
что и требовалось доказать.

>**Критерий Эйлера**
>Пусть $НОД(a, p) = 1, p > 2$ - простое. Тогда
>$\left( \frac{a}{p} \right) = 1 \iff a^{\frac{p-1}{2}} \equiv_{p} 1$

*Примечание*: 
$a^{p-1} \equiv_{p} 1 \iff ( a^ \frac{p-1}{2} - 1)( a^ \frac{p-1}{2} + 1) \equiv_{p}0 \implies$ либо $a^ \frac{p-1}{2} \equiv_{p} 1$, либо $a^ \frac{p-1}{2} \equiv_{p} -1$
Тогда, если, $\left( \frac{a}{p} \right) = 1 \iff a^{\frac{p-1}{2}} \equiv_{p} 1$, то верно и отрицание: $\left( \frac{a}{p} \right) = -1 \iff a^{\frac{p-1}{2}} \equiv_{p} -1$

*Доказательство*
(**=>**) $\left( \frac{a}{p} \right) = 1\implies \ \exists x: a \equiv_{p}x^2 \implies a^{\frac{p-1}{2}} \equiv_{p} x^\frac{(p-1) * 2}{2} \equiv_{p} x^{p-1} \equiv_{p} 1$ по малой теореме Ферма
**(<=)** Пусть $\left( \frac{a}{p} \right) = -1$. Докажем, что $\left( \frac{a}{p} \right) = 1 \iff a^{\frac{p-1}{2}} \not\equiv_{p} 1$.

Пусть 
$v=П_{v_{i}\in V}v_{i}$ - произведение всех квадратичных вычетов по модулю $p$.
$n=П_{n_{i}\in N}n_{i}$ - произведение всех квадратичных невычетов по модулю $p$.

$av_{1}\equiv_{p}n_{1}, av_{2} \equiv_{p}n_{2}, \dots, av_{\frac{p-1}{2}} \equiv_{p}n_{\frac{p-1}{2}}$
Тогда $a^ \frac{p-1}{2} \equiv_{p} n$