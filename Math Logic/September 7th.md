>[!info] Высказывание
>Строка сформулированная по следующим правилам:
>1. **Атомарное высказывание** - пропозициональная переменная: $A, B', C_1$
>2. **Составное высказывание**: если $\alpha$ и $\beta$ - высказывания, то высказываниями являются: 
>	- **Отрицание**: $\neg \alpha$
>	- **Конъюкция**: $\alpha \wedge \beta$
>	- **Дизъюнкция**: $\alpha \vee \beta$
>	- **Импликация**: $\alpha \rightarrow \beta$ или $\alpha \supset \beta$

>[!note] Соглашения о записи (метаязык)
>- **Метапеременные**: $\alpha, \beta, \gamma$ - маленькие греческие буквы
>- **Пропозициональная переменная**: $A, B, C$ - большие латинские буквы

### Оценка переменных
>[!info] Множество истинностных значений
>$$V = {И, Л}$$
>по сути булеан

>[!info]  Функция оценки перееменных (интерпритация)
>$$f: P \rightarrow V$$

>[!info] Общезначимая переменная (тавтология)
>Переменная, не зависещая от других переменных
>$$\models \alpha$$

>[!info] Гипотеза
>Выражение, истинное при истинности других переменных
>$$\gamma_1 \dots \gamma_n \vdash \alpha$$
>- если $\alpha$ истина при некоторых $\gamma_i$, то $\alpha$ - **выполнима**
>- если $\alpha$ ложно при любых $\gamma_i$, то $\alpha$ - **невыполнима**
>- если $\alpha$ ложно при некоторых $\gamma_i$, то $\alpha$ - **опровержима**

### Теория доказательств

>[!info] Схема высказывания
>Строка, построенная по правилам для построения высказываний

>[!tip] Аксиомы исчисления высказываний
>1. $\alpha \rightarrow \beta \rightarrow \alpha$
>2. $(\alpha \rightarrow \beta) \rightarrow (\alpha \rightarrow \beta \rightarrow \gamma) \rightarrow (\alpha \rightarrow \gamma)$ 
>3. $\alpha \rightarrow \beta \rightarrow \alpha\wedge\beta$
>4. $\alpha\wedge\beta \rightarrow \alpha$
>5. $\alpha\wedge\beta \rightarrow \beta$
>6. $\alpha \rightarrow \alpha \vee \beta$
>7. $\beta \rightarrow \alpha \vee \beta$
>8. $(\alpha \rightarrow \gamma) \rightarrow (\beta \rightarrow \gamma) \rightarrow (\alpha \vee \beta \rightarrow \gamma)$
>9. $(\alpha \rightarrow \beta) \rightarrow (\alpha \rightarrow \neg \beta) \rightarrow \neg \alpha$
>10. $\neg \neg \alpha \rightarrow \alpha$

>[!tip] Правило вывода Modus Ponens
>$$(\alpha \wedge (\alpha \rightarrow \beta)) \rightarrow \beta$$

>[!info] Доказательство
>Конечная последовательность высказываний, где каждое высказывания является:
>- Аксиомой
>- Получается из предыдущих по правилу Modus Ponens
>>[!example]
>>![[Pasted image 20240907200829.png]]

>[!info] Доказательство из гипотез
>Конечная последовательность высказываний, где каждое высказывания является:
>- Аксиомой
>- Получается из предыдущих по правилу Modus Ponens
>- Гипотезой

### Корректность и полнота

>[!info] Корректность теории
>Теория корректна, если любое доказуемое в ней утверждение общезначимо
>$$\vdash \alpha \Rightarrow \;\models \alpha$$ 

>[!info] Полнота теории
>Теория полна, если люьое общезначимое в ней утверждение доказуемо
>$$\models \alpha \Rightarrow \; \vdash \alpha$$ 

>[!done] Общезначимость правила Modus Ponens
>![[Pasted image 20240907201950.png]]