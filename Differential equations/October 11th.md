



>[!info] Нормальная система
>$$
\left\{ \begin{array} 
&  y'_{1} = f_{1}(t, y_{1}, y_{2},  \dots, y_{n}) \\ y'_{2} = f_{2}(t, y_{1}, y_{2},\dots, y_{n}) \\  \vdots \\ y'_{n} = f_{n}(t, y_{1}, y_{2},  \dots, y_{n})\end{array}\right.$$

>[!info] Решение системы ДУ
>$\varphi: E \to \mathbb{R}^{n}$, такая что:
>1. $\varphi\in C^{(1)}(E \to \mathbb{R}^{n})$
>2. $\varphi' = f(t, \varphi(x))$ на $E$

>[!note] 
>$$\Lambda_{n}\varphi = \left( 
>\begin{array}{c}\varphi \\ \varphi' \\ \vdots \\ \varphi^{(n)}
>\end{array}\right)$$


>[!lm] Лемма о нормальной системе равносильной уравнению высшего порядка
>$\operatorname{let} \varphi$ - решение [[October 4th#^7d4411|уравнения n-порядка]] на $E$
>$\Lambda_{n}\varphi$ - решение системы на $E$
>$$
\left\{ \begin{array}{lll}
y'_{1} = y_{2}, \\ y'_{2} = y_{3} \\  \vdots \\ y'_{n-1} = y_{n}\\ y'_{n} = f(t, y_{1}, y_{2},  \dots, y_{n})\end{array}\right.$$
Тогда $\psi = \left( \begin{array}{c} \varphi \\ \varphi_{1} \\ \vdots \\ \varphi_{n-1} \end{array} \right)$ на $E$, при чем $\psi = \Lambda_{n}\varphi$
>>[!proof]
>>1. $\operatorname{let} \varphi$ - решение уравнения на $E$, потдставим $\Lambda_{n}\varphi$ - в систему: $$\left\{ \begin{array}{lc} \varphi' = \varphi' & \text{- верно} \\ (\varphi')' = \varphi'' & \text{- верно} \\ \vdots \\ (\varphi^{(n-1)})' = f(t,  \varphi, \varphi', \dots, \varphi^{(n-1)}) & \text{- верно, так как } \varphi \text{ - решение уравнения}\end{array}\right.$$
>>2. $\operatorname{let} \psi$ - решение системы на $E$ $$\left[ y^{(n)} = f(t, y, y', \dots, y^{(n-1)})\right]_{y=\varphi} $$ $$\varphi^{(n)} = f(t, \varphi, \varphi' , \dots, \varphi^{(n-1)})$$ $$\varphi^{(n)} = f(t, \varphi, \varphi_{1}, \dots, \varphi_{n-1}) \text{ - верно из последнего равенства системы}$$

>[!info] Липшицево уравнение
>$f: D \to \mathbb{R}^{n}$, говорят что уравнение удовлетворяет условию Липшица $$f \in \operatorname{Lip} D$$ если $$\exists \; L > 0 : \forall \; r_{1}, r_{2} \in D \;\;\; |f(r_{1}) - f(r_{2})| \leq L|r_{1} - r_{2}| $$

>[!info] Локальная липшицевость
>$f:D\to \mathbb{R}^{n}, \;\; f \in \operatorname{Lip_{loc}(D)} \Leftrightarrow \;\forall \; r \in D \;\exists\; U_{r}: f \in \operatorname{Lip(U_{r}\cap D)}$

>[!info] Липшицевость по части переменных
>$f \in \operatorname{Lip}_{r_{1}}(D)$

--- 
>[!th] Теорема Пеано
>Пусть $f(t, x)$ - непрерывна по совокупности своих переменных в некоторой области.
>$a \geq |t - t_{0}|, \;\; b \geq |x - x_{0}|, \;\; \beta = max |f(t, x)|$ - в этой области, $h = min(a, \frac{b}{\beta})$, тогда на $[t_{0}- h, t_{0}+ h] \; \exists  \;$ хотя бы одно решение уравнения $\frac{dx}{dt}= f(t, x)$, удовлетворяющее начальному условию $x(t_{0})= x_0$