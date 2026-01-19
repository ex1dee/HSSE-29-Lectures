### 1

1. $$
\begin{array}c
\alpha e_{1} + \beta e_{2} = e_{1}' \\
\begin{cases}\alpha + \beta = 2 \\
\beta=1\end{cases} \implies \alpha = 1 \\
\alpha'e_{1} + \beta'e_{2} = e_{2}' \\
\begin{cases}\alpha+\beta=1 \\
\beta =2\end{cases} \implies \alpha = -1 \\
Получаем: \begin{cases}e_{1} + e_{2} = e_{1}' \\
-e_{1} + 2e_{2} = e_{2}'\end{cases} \\
C = \begin{pmatrix}
1  & -1 \\
1 & 2
\end{pmatrix}
\end{array}
$$
2. $$
\begin{array}c
\text{Пусть } a(x_{1}, y_{1}) \to a(x_{1}', y_{1}'), b(x_{2}, y_{2}) \to b(x_{2}', y_{2}') \\
a = \begin{pmatrix}
1 & -1 \\
1 & 2
\end{pmatrix} \cdot \begin{pmatrix}
3 \\
-1
\end{pmatrix} = \begin{pmatrix}
4 \\
1
\end{pmatrix} \\
b = \begin{pmatrix}
2 \\ 
3
\end{pmatrix} = \begin{pmatrix}
1 & -1 \\
1 & 2
\end{pmatrix} \cdot \begin{pmatrix}
x_{2}' \\
y_{2}'
\end{pmatrix} \\
\text{Найдём матрицу, обратную } C \\
C = \left(\begin{array}{cc|cc}
1 & -1 & 1 & 0 \\
1 & 2 & 0 & 1
\end{array}\right) = \left(\begin{array}{cc|cc}
1 & -1 & 1 & 0 \\
0 & 3 & -1 & 1
\end{array}\right) = \left(\begin{array}{cc|cc}
1 & 0 & -\frac{1}{3} & \frac{4}{3} \\
0 & 3 & -1 & 1
\end{array}\right) = \left(\begin{array}{cc|cc}
1 & 0 & -\frac{1}{3} & \frac{4}{3} \\
0 & 1 & -\frac{1}{3} & \frac{1}{3}
\end{array}\right) \\
C^{-1} = \begin{pmatrix}
-\frac{1}{3} & \frac{4}{3} \\
-\frac{1}{3} & \frac{1}{3}
\end{pmatrix} \\
b = C^{-1}\cdot\begin{pmatrix}
2 \\
3
\end{pmatrix} = \begin{pmatrix}
\frac{10}{3} \\
\frac{1}{3}
\end{pmatrix} \\
 \\

\end{array}
$$

### 2
