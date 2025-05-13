## 3
>[!done] 3 
>$$\forall\; W_{i}, W_{j} : W_{i} \preceq W_{j}, W_{i} \Vdash \alpha \text{ выполнено } W_{j} \Vdash \alpha $$
>>[!proof]
>>Раскроем $\alpha$:
>>$X)$ $$\; W_{i} \Vdash X \text{, то } W_{j} \Vdash X \text{ по определению}$$
>>$\alpha \& \beta)$ $$W_{i} \Vdash \alpha \& \beta \Rightarrow W_{i} \Vdash \alpha \;\&\; W_{i} \Vdash \beta \Rightarrow W_{j} \Vdash \alpha \;\&\; W_{j} \Vdash \beta \Rightarrow W_{j} \Vdash \alpha \& \beta \text { по определению}$$
>>$\alpha \vee \beta)$ $$ W_{i} \Vdash \alpha \vee \beta \Rightarrow W_{i} \Vdash \alpha \vee W_{i} \Vdash \beta \Rightarrow W_{j} \Vdash \alpha \vee W_{j} \Vdash \beta \Rightarrow W_{j} \Vdash \alpha \vee \beta \text { по определению}$$
>>$\alpha \to \beta)$ $$W_{i}\Vdash \alpha\to \beta \Rightarrow \forall W : W_{i} \preceq W \;\&\; W \Vdash \alpha \text{ выполнено } W \Vdash \beta$$ $$\forall W :  W_{j} \preceq W\;\; W_{i} \preceq W \text{ в силу транзитивности } \preceq$$
>>$$\Rightarrow \forall W : W_{j} \preceq W \;\&\; W \Vdash \alpha \text{ выполнено } W \Vdash \beta \Rightarrow W_{j}\Vdash \alpha\to \beta$$
>>$\neg \alpha)$ $$W_{i} \Vdash \neg \alpha \Rightarrow \forall W : W_{i} \preceq W \text{ выполнено } W \cancel{\Vdash} \alpha $$  $$\forall W :  W_{j} \preceq W\;\; W_{i} \preceq W \text{ в силу транзитивности } \preceq$$ $$\Rightarrow \forall W : W_{j} \preceq W \text{ выполнено } W \cancel{\Vdash} \alpha \Rightarrow W_{j} \Vdash \neg \alpha$$
