>[!info] Дифференцируемость
>$$f : E \subseteq \mathbb{R}^n \rightarrow \mathbb{R}^m,\;\; a \in \operatorname{Int}E$$
>$$f \in D \Leftrightarrow f(x) - f(a) = L(x - a) + o(||x-a||)$$

>[!info] Дифференциал
>Дифференциал в точке $a$: $L(x - a)$

>[!info] Частная производная
>$$\frac{\partial f}{\partial x_k}(a_1, \dots a_n) = \lim_{\Delta x \to 0} \frac{f(a_1, \dots, a_k + \Delta x, \dots, a_n) - f(a_1, \dots, a_n)}{\Delta x}$$

>[!info] Матрица Якоби
>Матрица Якоби - матрица производного оператора(дифференциала), имеет вид
>$$\begin{pmatrix}
{\partial f_1 \over \partial x_1}(x) & {\partial f_1 \over \partial x_2}(x) & \cdots & {\partial f_1 \over \partial x_n}(x) \\
{\partial f_2 \over \partial x_1}(x) & {\partial f_2 \over \partial x_2}(x) & \cdots & {\partial f_2 \over \partial x_n}(x) \\
\vdots & \vdots & \ddots &\vdots \\
{\partial f_m \over \partial x_1}(x) & {\partial f_m \over \partial x_2}(x) & \cdots & {\partial f_m \over \partial x_n}(x)
\end{pmatrix}$$
	
>[!done] Правило дифференцирования композиции
>$$] \; f: X \to Y, \;\; \varphi : U \to X, \;\; h : U \to Y\;\;\;h = f \circ \varphi$$
>$$d_{u_0}(f\circ\varphi) = d_{x_0}(f) \cdot d_{u_0}(\varphi)$$
>![[Pasted image 20240909130733.png]]

---
>[!info] Мультиндекс
>Целочисленный неотрицательный индекс
>$$\alpha \in (\mathbb{Z}_+)^n$$
>>[!done] Операции с мультиндексом
>>- $\alpha = (\alpha_1, \alpha_2, \dots, \alpha_n)$
>>- $|\alpha| = \alpha_1 + \alpha_2 + \dots + \alpha_n$ - длина
>>- $\alpha! = \alpha_1 \cdot \alpha_2 \cdot \dots \;\cdot \;\alpha_n$ - факториал
>>- $\operatorname{let} \; h \in \mathbb{R}^n \;\;\; h^{\alpha} = h_1^{\alpha_1}  \cdot \; \dots \; \cdot h_n^{\alpha_n}$ - возведение в степень
>>- $\operatorname{let} f:\mathbb{R}^n \to \mathbb{R}^m \;\; f^{(\alpha)}(a) = \frac{\partial^{(|\alpha|)}f}{\partial x_1^{\alpha_1}\dots \;x_n^{\alpha_n}}(a)$ - дифференцирование

>[!done] Lemma
>$$\operatorname{let}P_\alpha(x) = x^\alpha, \;\; \forall \; \alpha, \beta \in (\mathbb{Z}_+)^n \;\;\;P_\alpha^{(\beta)}(x) = \left\{ \begin{array}{rcl} 0 & \alpha \neq \beta \\ \alpha! & \alpha = \beta \end{array}\right.$$

>[!done] Lemma
>Если $\displaystyle\sum_{\alpha \in \mathbb{Z}_+^n} C_\alpha x^\alpha = p(x)$ - конечная сумма; $C_\alpha \in \mathbb{R}$, то $p^{(\beta)}(0) = C_\beta \beta! \Rightarrow C_\beta = \frac{P^{(\beta)}(0)}{\beta!}$ коэффициенты$(C_\xi)$ определены единственным образом

>[!theorem] Полиномиальная формула Ньютона
>$\operatorname{let} x = (x_1, \dots, x_n) \in \mathbb{R}^n\;\;\;\; r \in \mathbb{Z}_+$
>$$(x_1 + \dots + x_n)^r = \sum_{\substack{\alpha \in \mathbb{Z}_{+}^{n} \\ |\alpha| = r}} \frac{r!}{\alpha!}x^\alpha$$

### Представление для высших дифференциалов
>[!theorem] 
>$f:E\subseteq\mathbb{R}^n\to\mathbb{R}, \;\;\; a \in \operatorname{Int}E, \;\;\; \exists \; d^r_af$
>$$d^r_af = \left(d_{x_1} \cdot \frac{\partial f}{\partial x_1} + \dots + d_{x_n} \cdot \frac{\partial f}{\partial x_n}\right)^r$$
>$$\sum_{\substack{\alpha \in \mathbb{Z}_{+}^{n} \\ |\alpha| = r}} \frac{r!}{\alpha!}f^{(\alpha)}(\alpha)(dx_1, \dots, dx_n)^\alpha$$

>[!example] 2 случая вычесления дифференциала $r$-го порядка композиции
>1. $g = f \circ \varphi, \;\; \varphi:t \to a  + th, \;\; a, h \in \mathbb{R}^n$
>$a \in \operatorname{Int} E, \;\; f:E\to\mathbb{R}, \;\; R \in \mathbb{Z}_+, \;\; \exists \; d^rf$ на $E$
>If $a + th \in E, \;\; d_{a + th}^r\;g = d_{a + th}^r\;f (h) = \displaystyle\sum_{\substack{\alpha \in \mathbb{Z}_+^n \\ |\alpha| = r}} \frac{f^{(\alpha)}(a + th)}{\alpha!}h^\alpha$


>[!hence] Формула Тейлора-Лагранжа для ФНП
>$f: O \subseteq \mathbb{R}^n \to  \mathbb{R}, \;\; f \in C^{r + 1}(O), \;\; r \in \mathbb{Z}_+; \;\; a \in O, h \in \mathbb{R}^n, [a, a+h] \subset O$ Тогда 
>	$$\exists \; \Theta \in (0, 1) : f(a+h) = \displaystyle\sum_{k=0}^r \frac{d^k_a f(h)}{k!} + \frac{d^k_{a + \Theta h} f(h)}{(r + 1)!} = \sum_{\substack{\alpha \in \mathbb{Z}_{+}^{n} \\ |\alpha| = r}} \frac{f^{\alpha}(a)}{\alpha!}h^\alpha + \sum_{\substack{\alpha \in \mathbb{Z}_{+}^{n} \\ |\alpha| = r + 1}} \frac{f^{\alpha}(a + \Theta h)}{\alpha!}h^\alpha$$

---
 