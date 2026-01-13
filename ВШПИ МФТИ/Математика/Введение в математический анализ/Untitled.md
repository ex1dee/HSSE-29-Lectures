1. Точка $x_{0}$ является локальным экстремумом функции $f(x)$, если $f'(x_{0}) = 0$
2. Везде функция непрерывна на $[a, b]$ и дифференцируема на $(a, b)$
	- Теорема Ролля: если $f(a) = f(b)$, то $\ \exists \xi \in [a, b] : f'(\xi) = 0$
	- Теорема Лагранжа: $\ \exists \xi \in [a, b] : \frac{f(a) - f(b)}{a - b} = f'(\xi)$
	- Теорема Коши (обобщает Лагранжа): $\ \exists \xi:[a,b]: \frac{f(a) - f(b)}{g(a) - g(b)} = \frac{f'(\xi)}{g'(\xi)}$
3. Если $\ \exists f^{(n)}(x_{0})$, то при $x \to x_{0}:$ $f(x) = \sum_{k=0}^{n} \frac{f^{(n)}(x_{0})}{k!}(x-x_{0})^n + o((x - x_{0})^n)$
4. Пусть $f(x), g(x)$ дифференцируемы на $(a, b)$. Тогда если $\lim_{ x \to a }f(x) = \lim_{ x \to a }g(x) = 0$ и $g'(x) \neq 0 \ \forall x\in(a, b)$, то $\lim_{ x \to a } \frac{f(x)}{g(x)} = \lim_{ x \to a } \frac{f'(x)}{g'(x)}$
5. Если ты не против, я запишу формулы Маклорена:
	- $e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \dots$
	- $\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \dots$
	- $\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \dots$
	- $\ln(1 + x) = x - \frac{x^2}{2} + \frac{x^3}{3} - \dots$
	- $(1 + x)^\alpha = 1 + \alpha x + \frac{\alpha(\alpha - 1)}{2}x^2 + \dots$