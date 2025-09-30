>**Лемма**
>$\ \forall x_{0}\in \mathbb{R} \ \forall\delta>0$ в $U_{\delta}$ содержится хотя бы одна рациональная и хотя бы одна иррациональная точка.

*Доказательство*
Зафиксируем произвольное $\delta>0$, зафиксируем точку $x_{0}$
Выберем $k \geq\left[ \frac{1}{\delta} \right] + 1 \implies \frac{1}{k} < \delta$
$I_{k_{m}} = \left[ \frac{m}{2k}, \frac{m+1}{2k} \right), \frac{m}{2k}$ определяет рациональные дроби $\ \forall k\in \mathbb{N}, \ \forall m\in \mathbb{Z}$
$\ \forall\delta>0 \ \exists m\in \mathbb{Z} : I_{k_{m}} \subset U_{\delta}(x_{0}) \implies \frac{m}{2k} \in U_{\delta}(x_{0})$

$\sqrt{ 2 } \in \mathbb{R}\setminus \mathbb{Q} \implies \frac{\sqrt{ 2 }}{4k} \in \mathbb{R}\setminus \mathbb{Q}$
$x_{m} = \frac{m}{2k} + \frac{\sqrt{ 2 }}{4k} \in I_{k_{m}} \implies x_{m}\not\in \mathbb{Q}, x_{m}\in U_{\delta}(x_{0})$

> **Следствие**: 
> $\ \forall x_{0}\in \mathbb{R}$ является предельной точкой как для $\mathbb{Q}$, так и для $\mathbb{R}\setminus \mathbb{Q}$
> В частности, $cl\mathbb{Q} = \mathbb{R} = cl(\mathbb{R}\setminus \mathbb{Q})$

>Если $X$ - абстрактное множество, то $f:X\mapsto \mathbb{R}$ - **функция**

>Пусть $f:\dot{U}_{\delta_{0}}(x_{0})\mapsto R, x_{0} \in \hat{\mathbb{R}}, A \in \hat{\mathbb{R}}$
>Замечание: если $x_{0} = \pm \infty$ или $x_{0} = \infty$, то проколотая окрестность
>Будем говорить, что $A$ - предел функции $f$ в точке $x_{0}$ и записывать
>это $\lim_{ x \to x_{0} }f(x)=A$, если 
>$\ \forall \epsilon > 0 \ \exists \delta(\epsilon) \in (0, \delta_{0}] : \ \forall x \in \dot{U}_{\delta(\epsilon)}(x_{0}) \to f(x) \in U_{\epsilon}(A)$ (*по Коши*)

>Пусть $x_{0} \in \hat{\mathbb{R}},$ последовательность $\{ x_{n} \}$ называется последовательностью Гейне, если
>1) $x_{n} \to x_{0}$, 
>2) $x_{n} \neq x_{0}$
>Будем говорить, что $A$ - предел функции $f$ в точке $x_{0}$, если
>$\ \forall$ последовательности Гейне $\{ x_{n} \} \in \dot{U}_{\delta_{0}}(x_{0}) :f(x_{n}) \to A, n \to \infty$

>**Эквивалентность определений предела по Гейне и Коши**

*Коши -> Гейне*

По Коши: $\ \forall \epsilon > 0 \ \exists \delta(\epsilon) \in (0, \delta_{0}] : \ \forall x \in \dot{U}_{\delta(\epsilon)}(x_{0}) \to f(x) \in U_{\epsilon}(A)$
Пусть $\{x_{n}\} \in \dot{U}_{\delta_{0}}(x_{0})$ - последовательность Гейне
Т.к. $\{ x_{n} \} \to x_{0}, n\to \infty\implies \ \forall\delta>0\ \ \exists N(\delta) \in \mathbb{N} : \ \forall n \geq N(\epsilon) \to x_{n} \in \dot{U}_{\delta}(x_{0})$. Применим это для $\delta(\epsilon)$
$\ \forall \epsilon >0 \ \exists N = N(\delta(\epsilon)) \in \mathbb{N} \ \forall n \geq \mathbb{N} \to x_{n} \in \dot{U}_{\delta(\epsilon)}(x_{0})\implies$ $\implies \ \exists \lim_{ n \to \infty } f(x_{n}) = A$, Но $\{ x_{n} \}$ выбрано произвольно $\implies$

*Гейне -> Коши*
Пусть по Гейне, но не по Коши.
Отрицание к определению Коши: $\ \exists\epsilon>0:\ \forall\delta>0\ \exists x\in \dot{U}_{\delta}(x_{0}) : f(x) \neq U_{\epsilon}(A)$
Будем использовать это условие при $\delta_{n}=\frac{1}{n}$.
$\ \exists \epsilon>0 : \ \forall n \in \mathbb{N} \ \exists x_{0} \in \dot{U}_{\frac{\delta_{0}}{n}}(x_{0}) : f(x_{0}) \not\in U_{\epsilon}(A)$
Получили последовательность Гейне $\{ x_{n} \} \subset \dot{U}_{\delta_{0}}(x_{0})$, при этом $f(x_{n}) \not\to A, n \to \infty$
$\ \exists\epsilon>0:\ \forall n\in \mathbb{N} \to f(x_{n}) \not\in U_{\epsilon}(A)$ - противоречие с определением по Гейне.

>**Предел по множеству**
>Пусть $X \subset \mathbb{R}, X \neq \emptyset, x_{0}$ - его предельная точка. 
>Будем говорить, что $A \in \hat{\mathbb{R}}$ - предел $f:X\mapsto \mathbb{R}$ в точке $x_{0}$ по
>множеству $X$, если 
>- $\ \forall\epsilon>0 \ \exists \delta(\epsilon)>0 : \ \forall x\in \dot{U}_{\delta(\epsilon)}(x_{0})\cap X \to f(x) \in U_{\epsilon}(A)$ (*по Коши*)
>- $\ \forall$ последовательности Гейне $\{ x_{n} \}$ в точке $x_{0} \to f(x_{n}) \to A, n\to \infty$ (*по Гейне*)
>
>записывать это: $\lim_{ x \to x_{0}, x \in X }f(x) = A$ ?

по гейне экв. по коши

>**Лемма**
>Пусть $E_{1}, E_{2} \subset \mathbb{R}$ - непустые множества.
>$x_{0}\in \mathbb{R}$ - предельная точка и для $E_{1}$, и для $E_{2}$
>Тогда $\ \exists \lim_{ x \to x_{0}, x \in E_{1}\cup E_{2} }f(x) \iff \ \exists \lim_{ x \to x_{0}, x \in E_{1} }f(x)$ и $\exists \lim_{ x \to x_{0}, x \in E_{2} }f(x)$ (\*)

*Доказательство*
**(=>)**
$\ \forall \epsilon > 0 \ \exists \delta(\epsilon) \in (0, \delta_{0}] : \ \forall x \in \dot{U}_{\delta(\epsilon)}(x_{0}) \to f(x) \in U_{\epsilon}(A)$
Т.к. $x_{0}$ - предельная точка и для $E_{1}$, и для $E_{2}$, то
$$
\begin{cases}
E_{1}\cap \dot{U}_{\delta(\epsilon)}(x_{0}) \neq \emptyset \\
E_{2}\cap \dot{U}_{\delta(\epsilon)}(x_{0}) \neq \emptyset
\end{cases} ?
$$
Заметим, что $\dot{U}_{\delta}(x_{0}) \cap (E_{1} \cup E_{2}) = (\dot{U}_{\delta}(x_{0}) \cap E_{1}) \cup (\dot{U}_{\delta}(x_{0}) \cap E_{2})$
Тогда ?
$\ \forall \epsilon > 0 \ \exists \delta(\epsilon) \in (0, \delta_{0}] : \ \forall x \in \dot{U}_{\delta(\epsilon)}(x_{0})\cap E_{1} \to f(x) \in U_{\epsilon}(A) \iff \lim_{ x \to x_{0}, x \in E_{1} }f(x) = A$
$\ \forall \epsilon > 0 \ \exists \delta(\epsilon) \in (0, \delta_{0}] : \ \forall x \in \dot{U}_{\delta(\epsilon)}(x_{0})\cap E_{2} \to f(x) \in U_{\epsilon}(A) \iff \lim_{ x \to x_{0}, x \in E_{2} }f(x) = A$

**(<=)**
Пусть (\*). Очевидно $x_{0}$ - предельная точка для $E_{1}\cup E_{2}$
$$
(*) \iff
\begin{cases}
\ \forall \epsilon > 0 \ \exists \delta_{1}  > 0: \ \forall x \in \dot{U}_{\delta_{1}}(x_{0})\cap E_{2} \to f(x) \in U_{\epsilon}(A) \\
\ \forall \epsilon > 0 \ \exists \delta_{2}  > 0: \ \forall x \in \dot{U}_{\delta_{2}}(x_{0})\cap E_{2} \to f(x) \in U_{\epsilon}(A)
\end{cases}
$$
Определим $\delta(\epsilon) = min(\delta_{1}(\epsilon), \delta_{2}(\epsilon)) > 0$
Тогда, используя (1), получаем, что $\ \forall x\in \dot{U}_{\epsilon}(x_{0}) \cap (E_{1}\cup E_{2}) \to f(x) \in U_{\delta}(A)$
$\ \forall\epsilon>0 \ \exists\delta(\epsilon): \ \forall x \in \dot{U}_{\delta(\epsilon)}(x_{0}) \cap (E_{1} \cup E_{2}) \implies \ \exists \lim_{ x \to x_{0}, x \in E_{1}\cup E_{2} }f(x)=A$
___
$$
\text{Функция Дирихле D(x)} =
\begin{cases}
1, x \in \mathbb{\mathbb{Q}} \ \\
0, x \in \mathbb{R} \setminus \mathbb{Q}
\end{cases}
$$
У этой функции нет предела ни в одной точке.
Пусть $x_{0} \in \mathbb{R}$ - фиксированная точка.
$\lim_{ x \to x_{0}, x \in \mathbb{R} }f(x) = 1, \lim_{ x \to x_{0}, x \in \mathbb{R} \setminus \mathbb{Q} }f(x) = 0 \implies \text{не } \exists \lim_{ x \to x_{0} }D(x)$

___
>**Лемма**
>Пусть $x_{0}\in \hat{R}, f:\dot{U}_{\delta_{0}}(x_{0})$
>$\ \forall$ последовательности Гейне $\{ x_{n} \} \subset \dot{U}_{\delta_{0}}(x_{0})$ в точке $x_{0} \ \exists A(\{ x_{n} \}) \in \hat{\mathbb{R}} : \lim_{ n \to \infty }f(x_{n}) = A(\{ x_{n} \})$
>Тогда $\ \exists A \in \hat{R} : A=A(\{ x_{n} \}) \ \forall$ последовательности Гейне

Пусть $\{ x_{n} \} \subset \dot{U}_{\delta_{0}}(x_{0})$, $\{ y_{n} \} \subset \dot{U}_{\delta_{0}}(x_{0})$ - 2 последовательности Гейне в точке $x_{0}$

Покажем, что $A(\{ x_{n} \}) = A(\{ y_{n} \})$
$$
z_{n}=
\begin{cases}
x_{k}, \text{ если n = 2k} \\
x_{k}, \text{ если n = 2k - 1}
\end{cases}
\ \forall n \in \mathbb{N}
$$
A({x_n}) - предел x_n
$\{ z_{n} \}_{n=1}^\infty$ - последовательность Гейне в точке $x_{0}$ $\implies \ \exists A(\{ z_{n} \}) \in \hat{R} : f(z_{n}) \to A, n\to \infty \implies \{ f(x_{k}) \}$ и  $\{ f(y_{k}) \}$- подпоследовательности $\{ f(z_{n}) \} \implies A(\{ x_{n} \}) = \lim_{ k \to \infty }f(x_{n}) = A(\{ z_{n} \}) = \lim_{ k \to \infty }f(y_{k}) = A(\{ y_{k} \})$
$\implies$ предел не зависит от выбора последовательности, *ч.т.д.*

>**Критерий Коши**
>Пусть 
>Функция $f$ имеет конечный предел в точке $x_{0} \iff$выполнено 
>условие Коши: $\ \forall$

Пусть $\ \exists A \in \mathbb{R} : \lim_{ n \to \infty }f(x_{n}) = A$

()
Пусть выполнено условие Коши.
Пусть $\{ x_{n} \}\subset U_{\delta_{0}}(x_{0})$ - произвольная последовательность Гейне
$\ \forall \delta>0 \ \exists N(\delta) \in \mathbb{N}: \ \forall n \geq N(\delta) \to x_{n} \in \dot{U}_{\delta}(x_{0})$
Взяв $\delta=\delta(\epsilon)$, получим: $\ \exists N=N(\delta(\epsilon)) \in \mathbb{N} : \ \forall n, m \geq N \to |f(x_{n}) - f(x_{m})| < \frac{\epsilon}{2}\implies$ последовательность $\{ f(x_{n}) \}$ удовлетворяет условию Коши $\implies$ в силу критерия Коши для последовательности, $\ \exists \lim_{ n \to \infty }f(x_{n}) = A \in \mathbb{R}$.
Но по предыдущей лемме, число $A$ не зависит от выбора последовательности Гейне $\implies$ выполнено определение по Гейне: $\ \exists A \in \mathbb{R}:\ \forall$ последовательности Гейне $\{ x_{n} \}\subset \dot{U}_{\delta_{0}}(x_{n})$ в точке $x_{0} \to \ \exists \lim_{ n \to \infty }f(x_{n})=A \implies$ по Гейне $\ \exists \lim_{ x \to x_{0} }f(x)=A\in \mathbb{R}$.

