$\bar{r} : [a, b] \to R^n$, $Г = \{ \bar{r}(t) : t \in [a, b] \}$

$\gamma : [c, d] \to [a,b]$, $t = \frac{\gamma}{2}$

$$
|Г| = sup_{разбиения} \sum_{i=1}^I |\bar{r}_{i} - \bar{r}_{i-1}|
$$

$$
k(t) = \frac{|\bar{r}'(t) \times \bar{r}''(t)|}{|\bar{r}'(t)|^3}
$$
$$
k(s) = |\bar{r}''(s)|
$$
$$
s: [a, b] \to [0, |Г|]
$$

$$
\sigma(s) = \bar{r}(t(s))
$$




$R = \frac{1}{k}$


$$
\begin{array}c
\tau(s) = r'(s) \text{ - касательная}\\ 
n(s) = \frac{\tau'(s)}{|\tau'(s)|} \text{ - главная нормаль}\\
b(s) = \tau(s) \times n(s) \text{ - бинормаль} \\
 \\
\tau(t) = \frac{r'(t)}{|r'(t)|} \\
b(t) = \frac{r'(t) \times r''(t)}{|r'(t) \times r''(t)|} \\
n(t) = \tau(t) \times b(t)
\end{array}
$$