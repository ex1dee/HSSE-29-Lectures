При фиксированных $k^* \in \mathbb{Z}$ и $m^* \in \mathbb{Z}$ найти количество двоичных кубов $Q_{k^*,m}$, имеющих общие точки с кубом $Q_{k^*, m^*}$

Условие пересечения: $\begin{cases}s^1 \leq e^2 \\ s^2 \leq e^1\end{cases}$

Пусть $Q_{k^*,m} = (s^1, e^1)$, $Q_{k^*, m^*} = (s^2, e^2)$

$s^1 = \left( \frac{m_{1}}{2^{k^*}}, \dots, \frac{m_{n}}{2^{k^*}} \right)$
$s^2 = \left( \frac{m^*_{1}}{2^{k^*}}, \dots, \frac{m^*_{n}}{2^{k^*}} \right)$

$e^1 = \left( \frac{m_{1} + 1}{2^{k^*}}, \dots, \frac{m_{n} + 1}{2^{k^*}} \right)$
$e^2 = \left( \frac{m^*_{1} + 1}{2^{k^*}}, \dots, \frac{m^*_{n} + 1}{2^{k^*}} \right)$

Условие пересечения: 
$$
\begin{cases} \frac{m_{i}}{2^{k^*}} \leq \frac{m_{i}^* + 1}{2^{k^*}} \\
\frac{m_{i}^*}{2^{k^*}} \leq \frac{m_{i} + 1}{2^{k^*}} \end{cases} \iff \begin{cases}m_{i} \leq m_{i}^* + 1 \\
m_{i}^* \leq m_{i} + 1\end{cases} \iff \begin{cases}m_{i} - m_{i}^* \leq 1 \\
m_{i} - m_{i}^* \geq -1\end{cases}
$$
$$
\iff |m_{i} - m_{i}^*| \leq 1
$$
Т.к. $m_{i}, m_{i}^* \in \mathbb{Z}$, то возможные значения $m_{i} - m_{i}^*$: $\{ -1,0, 1 \}$. При фиксированном $m_{i}^*$ макс. кол-во $m_{i}$ равно 3

Следовательно, ответ: $3^n$