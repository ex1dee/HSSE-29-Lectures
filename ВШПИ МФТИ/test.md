Ну вот хочу найти константу $C_{1} : C_{1}\sum|x_{k}| \leq ||x||$
Фиксирую $x$. Нахожу $C_{x}: C_{k}\sum|x_{k}| \leq ||x||$
Если$\sum|x_{k}| = 0$, то берем любой $C_{x}$, пусть $C_{x} = 1$
$C_{x} \leq \frac{||x||}{\sum|x_{k}|}$
$\frac{1}{C_{x}} \geq \frac{\sum|x_{k}|}{||x||}$
Пусть $\frac{1}{C_{x}} = \frac{\sum|x_{k}|}{||x||} + 1 \implies C_{x} = \frac{1}{\frac{\sum|x_{k}|}{||x||} + 1}$

И тогда $C_{1} = min_{x\in V} C_{x}$

$\frac{\sum|x_{k}|}{||x||} + 1 \geq 1 \implies C_{x} \geq 1 \implies C_{1} > 0$

Из оценки сверху: $\frac{||x||}{\sum|x_{k}|} \leq M \in \mathbb{R}$
Докажем оценку снизу: $\ \exists C_{1}>0: \ \forall x \in V \to C_{1}\sum|x_{k}| \leq ||x||$
От противного: $\ \forall C_{1} >0 \to  \ \exists x \in V :  C_{1}\sum|x_{k}| > ||x||$

$C_{n} = \frac{1}{n}$
$\ \forall n \in \mathbb{N} \ \exists x^{n}\in V: ||x^n|| < \frac{1}{n} \sum|x^n_{k}| \iff \frac{||x^n||}{\sum|x^n_{k}|} < \frac{1}{n}$