>[!info] 
>Система $\mathcal{F}$ подмножеств $\Omega$ (мн-ва элементарных исходов) называется **$\sigma$ - алгеброй**, если
>1. $\Omega \in \mathcal{F}$
>2. $A\in \mathcal{F} \Rightarrow \mathcal{F} \setminus A \in \mathcal{F}$
>3. $\displaystyle\bigcup_{i=1}^{\infty} A_{i} \in \mathcal{F}$

>[!note] 
>4. $2), 3) \Rightarrow 1)$
>5. $A, B \in \mathcal{F} \Rightarrow A \setminus B \in \mathcal{F}$

>[!info] Вероятность
>$\operatorname{let} \Omega$ - пространство элементарных исходов, $\mathcal{F}$ - его $\sigma$ - алгебра. **Вероятностью** на $\left<\Omega, \mathcal{F}\right>$ называется функция $P:\mathcal{F} \to \Omega$, такая что:
>1. $\forall \; A \in  \mathcal{F} \;\;\; P(A) \geq 0$
>2. Если $A_{1}, \dots, A_{n} \in \mathcal{F}$ попарно несовместны, то $P\left(\sum\limits_{i=1}^{\infty} A_{i}\right) = \sum\limits_{i=1}^{\infty}P(A_i)$
>3. $P(\Omega) = 1$

>[!note]
>$P$ - нормированая мера

>[!Lm] 
>1. $P(\varnothing) = 0$
>2. $\forall\; A \in \Omega\;\;\;0 \leq P(A) \leq 1$

### Аксиома непрерывности

>[!tip] Аксиома непрерывности
>$\operatorname{let} A_{1} \subset A_{2} \subset A_{3} \subset \dots$
>$\displaystyle\bigcap_{i =1}^{\infty} A_{i} \neq \varnothing$
>Тогда $P(A_{n}) \to 0$

>[!th]
>Аксиома непрерывности следует из счетной аддитивности


>[!tldr] Свойства вероятности
>1. Дистрибутивность $A \cdot (B + C) = A \cdot B + A \cdot C$
>2. $\operatorname{let}A, B$ несовмесны, тогда $P(A + B) = P(A) + P(B)$