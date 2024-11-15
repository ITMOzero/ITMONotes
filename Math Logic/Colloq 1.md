>[!info] Топологическое пространство
>Упорядоченная пара $(X, \Omega)$, где $X$ множество, $\Omega$ - топология
>**Топология** - $\Omega \subseteq 2^X:$
>- $\varnothing, X \in \Omega$
>- $\forall \; U_\alpha$ - семейства в $\Omega \;\;\; \displaystyle\bigcup_\alpha U_\alpha \in \Omega$
>- $\forall \; \left\{U_i\right\}_{i = 1}^{n} \in Omega \;\;\; \displaystyle\bigcap_{i = 1}^n U_i \in \Omega$

>[!info] Метрическое пространство
>Упорядоченная пара $(X, \rho)$, где $X$ множество, $\rho$ - метрика
>**Метрика** - $\rho:X^2 \to \mathbb{R}:$
>- $\forall \; x, y \in X \; \; \rho(x, y) \geq 0 \;\;\;\; \rho(x, y) = 0 \Leftrightarrow x = y$
>- $\forall \; x, y \in X \; \; \rho(x, y) = \rho(y, x)$
>-  $\forall \; x, y, z \in X \;\; \rho(x, y) + \rho(y, z) \geq \rho(x, z)$

>[!example]
>>[!info] Топология стрелки
>>$$X = \mathbb{R}\;\;\;\; \Omega = \left\{[a, b) : a, b \in \mathbb{R}, a < b\right\}$$
>
>>[!info] Топология на деревьях
>>Дан лес, на деревьях введено отношение $\preceq : a \preceq b \Leftrightarrow b$  - потомок $a$, тогда в топологии будут содержаться поддеревья, в которых каждая вершина содержит всех своих потомков
>>![[Pasted image 20241023205608.png]]

>[!info] Открытые множества
>Множество $M$ открыто в $X$ если $M \in \Omega$

>[!info] Замкнутые множества
>Множество $M$ замкнуто в $X$ если его дополнение открыто
>$$X \setminus M \in \Omega$$

>[!info] Связные множества
>Пространство $\left<X, \Omega\right>$ - связно, если $$\not\exists A, B \in \Omega : A \cup B = X, A \cap B = \varnothing$$
>>[!example]
>>![[Pasted image 20241023211036.png]]

>[!info] Компактность
>Множество компактно если из любого его открытого покрытия можно выделить конечное подпокрытие 


---

>[!info] Решетка
>Упорядоченная пара $\left<X, \preceq\right>$, где $X$ - множество, $\preceq$ - отношение частичного порядка, такое что $\forall \; a, b \in X$ определены $a + b =  \sup\{a, b\}, a \cdot b = \inf\{a, b\}$

>[!info] Псевдодополнение
>$a \to b = \max(x : a \cdot x \preceq b)$ 

>[!info] Дистрибутивная решетка
>Решетка в которой $$\forall \; a, b, c \in X \;\;\; a \cdot (b + c) = a \cdot b + a \cdot c$$

>[!info] Импликативная решетка
>Решетка в которой $$\forall \; a, b \in X \;\; \exists \; a \to b$$

>[!done] Lemma
>Импликативная решетка дистрибутивна 

>[!info] Наибольший и наименьший элемент решетка
>$1$ - наибольший элемент решетки
>$0$ - наименьший элемент решетки

>[!done] Lemma
>В импликативной решетке $\exists \;1$
>>[!important] Proval
>>$$\measuredangle \; a \to a = \max\{x : a \cdot x \preceq a\} = \max(X) = 1$$

>[!info] Псевдобулева алгебра
>Импликативная решетка с $0$
>В такой решетке определено $\sim a := a \to 0$

>[!info] Булева алгебра
>Псевдобулева алгебра в которой $$\forall \; a\in x \;\;\;\; a + \sim a = 1$$

>[!done] Lemma
>![[Pasted image 20241023214919.png]]

>[!example]
>![[Pasted image 20241023215321.png]]

---
![[Pasted image 20241023215400.png]]

>[!info] Алгебра Линденбаума
>![[Pasted image 20241023215507.png]]

![[Pasted image 20241023215530.png]]