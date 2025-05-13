$S_{i} \in \{\{0\}, \{1\}, [0, 1]\}$, $|\{0\}| = |\{1\}| = 0$, $|[0, 1]| = 1$ - веса (влияние на размерность)
$$a_{nm} = {n \choose k} 2^{n-m} \text{  - колличество граней размерности m в n - мерном гиперкубе}$$
$$A(u, z) = \sum\limits_{n}\sum\limits_{m = 0}^{n}a_{nm}u^{m}z^{n} = \sum\limits_{n}\sum\limits_{m = 0}^{n}{n \choose k} 2^{n-m}u^{m}z^{n} = \sum\limits_{n}z^{n} \left(\sum\limits_{m = 0}^{n}{n \choose k} 2^{n-m}u^{m}\right)$$
$$\sum\limits_{m = 0}^{n}{n \choose k} 2^{n-m}u^{m} = \left[(\alpha+\beta)^{t} = \sum\limits_{k=0}^{t}{t\choose k}\alpha^{t-k}\beta^{k}, \;\; \alpha := 2, \beta := u, t := n, k:= m\right] = (2 + u)^{n}$$
$$A(u, z) = \sum\limits_{n}z^{n}(2 + u)^{n} = \frac{1}{1-(2+u)z}$$
