$$
\lim_{ x \to 0 } \frac{(ch x)^{\sin \sin \frac{3x}{4}} - (chx)^{shshx}}{\arcsin tgx - \sin arctgx}
$$
$$
\begin{array}c
\sin \frac{3x}{4} = \frac{3x}{4} - \frac{9x^3}{128} + o(x^3) \\
\sin \sin \frac{3x}{4} = \frac{3x}{4} - \frac{9x^3}{128} - \frac{27x^3}{64}=\frac{3x}{4}-\frac{63x^3}{128}+o(x^3) \\
ch x = 1 + \frac{x^2}{2} + o(x^3) \\
\ln(chx) = \ln\left( 1 + \frac{x^2}{2} + o(x^3) \right) = \frac{x^2}{2} + o(x^3)\\
\frac{1}{1 + x} = 1 - x + x^2 + o(x^2) \\
(chx)^{\sin \sin \frac{3x}{4}} = e^{\sin \sin \frac{3x}{4} \cdot \ln(chx)} = e^{\left( \frac{3x}{4}-\frac{9x^3}{64} \right)\left( \frac{x^2}{2} - \frac{x^{4}}{12} \right) + o(x^3)=e^{\frac{3x^3}{8} + o(x^3)}}, \lim_{ x \to 0 } e^{\frac{3x^3}{8}+o(x^3)}=e^{0} = 1 \\
 \\
sh x = x  + \frac{x^3}{3} + o(x^3) \\
sh sh x = x + \frac{2x^3}{3} + o(x^3) \\
(chx)^{shshx} = e^{}
\end{array}
$$

$$
\begin{array}c
tg x =  \\
= \frac{\sin x }{\cos x} = \frac{x - \frac{x^3}{6}}{1 - \frac{x^2}{2}} = \left( x - \frac{x^3}{6} \right)\left( 1 + \frac{x^2}{2} \right) + o(x^3) = x + \frac{x^3}{2} - \frac{x^3}{6} + o(x^3) = x + \frac{x^3}{3} + o(x^3)  \\
\arcsin tg x = x + \frac{x^3}{6} + o(x^3) \\
\frac{1}{\sqrt{ 1 - x^2 }} = (1 - x^2)^{\frac{1}{2}} = 1 + \frac{x^2}{2} + o(x^2) \\
 \\
arctgx = x - \frac{x^3}{3} + o(x^3) \\
\frac{1}{1 + x^2} = 1 - x^2 + o(x^2) \\
\sin arctgx = x - \frac{2x^3}{3} + o(x^3) \\
g(x) = \frac{5x^3}{6} + o(x^3)
\end{array}
$$