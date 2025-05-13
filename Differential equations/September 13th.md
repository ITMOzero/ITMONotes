### Общее решение уравнения с разделенными переменными

>[!info] Общее решение уравнения с разделенными переменными
>$$\operatorname{let}  \; \; E_x \subset O_x \;\; E_y \subset O_y \; ;\; P \in C(E_x),\; Q \in C(O_y),\; E = \left<a, b\right> \subset O_x$$
>Тогда функция $\varphi:E \to \mathbb{R}$ - решение [[September 6th#^83f701|уравнения]] тогда и только тогда, когда 
>1. $\varphi \in C'(E)$
>2. $\int P(x)dx + \int Q(y)dy \equiv C$

### Уравнение с разделяющимися переменными
>[!info] Уравнение с разделяющимися переменными
> Уравнение вида: $$P_1(x)Q_1(y)dx + P_2(x)Q_2(y)dy = 0$$

>[!theorem] Общая схема исследования общего решения уравнения с разделяющимися переменными
>$$xdy - 2ydx = 0 \;\;\;\; (*)$$
>$$\operatorname{dom} (*) = \mathbb{R}^2$$
>$$\frac{dy}{y} = \frac{2dx}{x} \;\;\;\; (**)$$
>$$\operatorname{dom} (**) = \mathbb{R}^2 \setminus \{O_x, O_y\}$$

### Линейные уровнения первого порядка

^ecb181

>[!info] Линейное уравнение первого порядка
>$$y' = p(x)y + q(x)$$

>[!info] Линейное однородное уравнение первого порядка
>$$y' = p(x)y$$

>[!theorem] Общее решение линейного уравнения первого порядка
>$p, q \in C(E)$, тогда общее решение имеет вид:
$$y = \frac{C + \int q \mu}{\mu} \;\;\;\;\; \mu = e^{-\int p} \;\;\;\;\; C \in \mathbb{R}$$
>>[!proof]
>>Пусть $S$ - множество всех решений
>>$F = \left\{\varphi: \tilde{E} \to \mathbb{R} \;|\; \tilde{E} \subset E, \;\;\; \varphi = \frac{C + \int q \mu}{\mu}\right\}$
>>$S\subseteq F:\;\; \operatorname{let} \varphi \in S, \;\;\; \operatorname{dom} (\varphi) = \tilde{E} \subset E$
>>$$\varphi'(x) = p(x)\varphi(x) + q(x)$$
>> $$\varphi'\mu = p\varphi\mu + q\mu$$
>> $$\varphi'\mu - p\varphi\mu = q\mu$$
>> $$\varphi' e^{-\int p} - p\varphi e^{-\int p} = q\mu$$
>> $$\left(\varphi e^{-\int p}\right)' = q\mu$$
>> $$\varphi e^{-\int p} = \int q\mu + C$$
>> $$\varphi = \frac{\int q\mu + C}{\mu} \;\;\;\Rightarrow \varphi \in F$$
>> $F \subseteq S: \;\;\; \operatorname{let } \varphi \in F$
>> Проделав действия в обратном порядке придем к
>> $$\varphi' = p\varphi + q \;\;\;\Rightarrow \varphi \in S$$
>> Значит $F = S$

>[!hence] Общее решение линейного однородного уравнения первого порядка
>$$y = Ce^{\int p} \;\;\;\; C \in \mathbb{R}$$