1. $y_{n} < +\infty \ \forall n \in \mathbb{N}$
$y_{n} = sup \{ x_{k}: k \geq n \} \ \forall n \in \mathbb{N}$

Последовательность $\{ y_{n} \}$ - монотонна => по теореме Вейерштрасса имеет предел, равный её инфимуму => $inf y_{n} = \lim_{  n \to \infty } y_{n}$
	$y_{n+1} \leq y_{n} \ \forall n \in \mathbb{N}$

2. $\\lim_{ n \to \infty } x_{n} \leq inf y_{n}$
Т.к. верхний предел является частичным пределом, то существует подпоследовательность $\{ x_{n_{j}} \} : \lim_{ j \to \infty } x_{n_{j}} = \overline{\lim}_{ n \to \infty} x_{n}$
$\ \forall j \in \mathbb{N} : x_{n_{j}} \leq y_{n_{j}}$, но $\lim_{ j \to \infty } y_{n_{j}} = inf y_{n} \implies$ перейдём к пределу в неравенстве (\*)
Получим $\overline{\lim}_{ n \to \infty} x_{n} \leq inf y_{n}$

3. Установим неравенство $\overline{\lim}_{ n \to \infty } x_{n} \geq inf y_{n} = inf sup_{k\geq n} x_{k}$. Достаточно доказать, что правая часть является частичным пределом $\{ x_{n} \}$.
По определению $inf: \ \forall \epsilon>0 \ \exists N_{e} : \ \forall n >N_{e} \to y_{n} \in U_{\frac{e}{2}}(M)$
По определению $sup_{k\geq n} x_{k}: \ \exists k > n : x_{k} \in U_{\frac{e}{2}(y_{n})}$

$U_{\frac{\epsilon}{2}(y_{n})} \subset U_{\frac{\epsilon}{2}(M)} \ \forall n \geq N(\epsilon)$ 
$\ \forall \epsilon > 0 \ \forall N \in \mathbb{N} \ \exists k = max(N, N_{\epsilon}) + 1 : x_{k} \in U_{e}(M)$ => по критерию частичного предела M - частичный предел => неравенство доказано.

> **Теорема о единственном частичном пределе**
> Пусть $\{ x_{n} \}$ - числовая последовательность и $A \in \overline{\mathbb{R}}$. Следующие условия эквивалентны:

1. $\ \exists \lim_{ n \to \infty } x_{n} = A$
2. Множество частичных пределов состоит из 1 элемента
3. $\underline{\lim}_{n\to \infty} x_{n} = \overline{\lim}_{n \to \infty} x_{n} = A$

*Доказательство*
(1) => (2) 
(3) => (1)

**(3) => 1**
Пусть $A \in \mathbb{R}$. 
$\underline{\lim}_{n\to \infty} x_{n} = sup inf_{k\geq n} x_{k}$.
$\overline{\lim}_{n\to \infty} x_{n} = inf sup_{k\geq n} x_{k}$.

$y_{n} = sup_{k\geq n}x_{k} \in \mathbb{R} \ \forall n \in \mathbb{N}$
$z_{n} = inf_{k\geq n}x_{k} \in \mathbb{R} \ \forall n \in \mathbb{N}$
Тогда $\{ y_{n} \}, \{ z_{n} \}$ - числовые последовательности
$\lim_{ n \to \infty } y_{n}$ = $\lim_{ n \to \infty } z_{n} = A$
$z_{n} \leq x_{n} \leq y_{n} \ \forall n \in \mathbb{N}$ => по т. о 2 миллиционерах $\ \exists \lim_{ n \to \infty } x_{n} = A$

Рассмотрим случай $A = +\infty$, для $A = -\infty$ аналогично.
	По условию $\underline{\lim}_{n\to \infty} x_{n} = +\infty = sup inf_{k\geq n} x_{k} =$, но $\{ z_{n} \}$ - монотонно возрастающая => по т. Вейерштрасса $\ \exists \lim_{ n \to \infty } z_{n} = _\infty$ $\ \forall \epsilon >0 \ \exists N_{e}: \ \forall n \geq N_{e}\to z_{n} > \frac{1}{e} \implies$ по определению $z_{n}$: $x_{k} > \frac{1}{e} \implies$ $\ \forall \epsilon>0 \ \exists N_{e} : \ \forall k \geq N_{e} \to x_{k} > \frac{1}{e}$

> Последовательность $\{x_{n}\}$ называется фундаментальной, если она удовлетворяет условию Коши:
> $\ \forall \epsilon>0 \ \exists N_{e} \in \mathbb{N} : \ \forall n, m \geq N_{e} \to |x_{n} - x_{m}| < \epsilon$

> **Лемма**
> $\{ x_{n} \}$ удовлетворяет условию Коши $\implies$ она ограничена

По условию Коши при $\epsilon = 1: \ \exists N_{1} : \ \forall n, m \geq N_{1} \to |x_{n} - x_{m}| < 1$
В частности, положив $m =N_{1}, получим, что $|x_{n} - x_{N_{1}}| < 1 \ \forall n \geq N_{1}$
Получается, что при $n \geq N_{1}$ по неравенству треугольника $|x_{n}| \leq |x_{n} - x_{N_{1}}| + |x_{N_{1}}| < 1 + |x_{N_{1}}|$

Определим $N = max(|x_{1}|, |x_{2}| \dots |x_{N_{1}}| + 1)$
Итого: $|x_{n}| \leq M \ \forall n \in \mathbb{N}$

> **Критерий Коши**
> $\{ x_{n} \}$ сходится $\iff$ она фундаментальна

*Необходимость*
Пусть $x_{n}$ сходится. Покажем, что выполнено условие Коши.
$\ \exists x \in \mathbb{R} : \lim_{ n \to \infty }x_{n} = x \iff$ 
$\ \forall \epsilon > 0 \ \exists N_{e} : \ \forall n \geq N_{e} \to |x - x_{n}| < \frac{\epsilon}{2}$
$\ \forall \epsilon > 0 \ \exists N_{e} : \ \forall n \geq N_{e} \to |x_{n} - x| < \frac{\epsilon}{2}$

=> $\ \forall n\geq N_{e} \ \forall m \geq= N_{e} \to |x_{n} - x_{m}| \leq |x_{n} - x| + |x - x_{n}| < 2 * \frac{\epsilon}{2} = \epsilon$

Итого: $\ \forall \epsilon > 0 \ \exists N_{e} : \ \forall n, m \geq N_{e} \to |x_{n} - x_{m}| < \epsilon$

*Достаточность*
Пусть $x_{n}$ сходится. Требуется доказать, что последовательность сходится
По лемме 1 $\{ x_{n} \}$ - ограниченная $\implies$  по т. Больцано-Вейерштрасса $\ \exists$ конечный частичный предел, т.е. $\ \exists x \in \mathbb{R}, \ \exists \{ x_{n_{k}} \} : x = \lim_{ k \to \infty } x_{n_{k}}$
$\lim_{ k \to \infty } x_{n_{k}}$: $\ \forall \epsilon > 0 \ \exists K_{e} : \ \forall n \geq K_{e} \to |x - x_{n_{k}}| < \epsilon$

$\ \forall \epsilon > 0 \ \exists N_{e} : \ \forall n, m \geq N_{e} \to |x_{n} - x_{m}| < \epsilon$
Пусть $L_{\epsilon} = max(N_{e}, K_{e})$. Если $k \geq L_{e}$, то $|x_{n_{k}} - x| < \epsilon$, $|x_{n} - x_{n_{k}}| < \epsilon \ \forall n \in \mathbb{N}$ и $k \geq N_{e}, n_{k} \geq k \geq N_{e}$.

$\ \forall \epsilon > 0 \ \exists N_{e} : \ \forall n \geq N_{\epsilon} \to |x - x_{n}| = |x \pm x_{n_{k}} - x_{n}|$, где $k \geq L_{e}$
$|x - x_{n_{k}}| + |x_{n_{k}} - x_{n}| < 2\epsilon$

Итого: $\ \forall \epsilon > 0 \ \exists N_{e} : \ \forall n \geq N_{e} \to |x_{n} - x| < 2\epsilon \implies \ \exists \lim_{ n \to \infty } x_{n} = x$

*Замечание: критерий Коши обычно используется, чтобы доказать расходимость*

>Пример: $x_{n} = (-1)^n, n \in \mathbb{N}$

Запишем отрицание к условию Коши: $\ \exists \epsilon > 0 : \ \forall N \in \mathbb{N} \ \exists n, m \geq N \to |x_{n} - x_{m}| \geq \epsilon$
$\ \exists \epsilon = 2 : \ \forall N \in \mathbb{N} \ \exists n = 2N \ \exists m = 2N + 1 \to |x_{n} - x_{m}| = 2 \geq \epsilon$

>Топология числовой прямой

> Пусть $E \subset \mathbb{R}$. Будем говорить, что точка $\underline{x} \in \mathbb{R}$ является точкой прикосновения $E$, если $\ \forall \epsilon > 0 \ U_{e}(\underline{x})\cap_{}E \neq 0$

>Множество называется замкнутым, если оно содержит все свои точки прикосновения. 

>Пусть $E \subset \mathbb{R}$ - множество. ??
>$E \subset clE$

>$E$ замкнуто $\iff$ $E = clE$

Пример: $[a, b]: -\infty < a < b < +\infty$
Если $x \neg in [a, b]$ $\epsilon =$? ???

>Пусть $E \subset \mathbb{R}$ - множество. Точка $x_{0} \in E$ - внутренняя, если $\ \exists \epsilon > 0 : U_{e}(x_{0}) \in E$. 

> Множество $G$ называется открытым, если каждая его точка является внутренней.

>Пусть $E \subset \mathbb{R}$ - множество. $int E$ - множество всех внутренних точек $E$
>$int E \subset E \iff$ E - открытое

Пример: $E = (a, b)$ - открытое множество
Берём $\ \forall x \in (a, b)$. $\ \exists \epsilon = min(|x - a|, |x - b|) : U_{e}(x) \subset (a,b)$ 

*Замечание: пустое множество и $\mathbb{R}$ замкнуты и открыты по определению.

Пример: $E = [a, b)$
$-\infty < a < b < +\infty$
E - не открыто. $U_{e}(a) \neg \subset [a, b) \ \forall \epsilon > 0$
С другой стороны, b - точка прикосновения множества E, но $b \neg \subset E$

$int E = (a, b)$, $clE = [a, b]$

>**Теорема**
>Пусть $\{ G_{\alpha} \}_{\alpha \in I}$ - произвольное семейство открытых множество ($I$ - индексное множество). Тогда $G = \cup_{a \in I} G_{x}$, $\{ F_{\beta} \}_{\beta \in J}$ - произвольное замкнутое множество, но

>**Лемма**
>$G \subset \mathbb{R}$ – открытое $\iff$ $\mathbb{R}\setminus G$ - замкнутое

Пусть 

 Пусть $x \in \cup_{\alpha}a_{\alpha} \implies \ \exists \underline{\alpha} : x \in G_{\underline{\alpha}}$, то $G_{\underline{\alpha}}$ - открытое $\implies \ \exists \epsilon >0 : U_{\epsilon(x)} \subset G_{\underline{x}} \subset \cup_{\alpha \in I} G_{\alpha} \implies$ т.к. x выбрано произвольно, то $\cup_{\alpha \in I}G_{x}$ - открытое. 

$\cap_{\beta \in I} F_{\beta} = \mathbb{R}\setminus(\cup_{\beta \in J}(\mathbb{R}\setminus F_{\beta}))$