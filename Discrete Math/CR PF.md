### Task 1
$$\sum\limits_{n}\sum\limits_{m}a_{n,m}x^{n}y^{m} = \sum\limits_{n}\sum\limits_{m}(n + m)x^{n}y^{m} = \sum\limits_{n}\sum\limits_{m}nx^{n}y^{m} + \sum\limits_{n}\sum\limits_{m}mx^{n}y^{m}$$
$$\sum\limits_{n}\sum\limits_{m}nx^{n}y^{m} = \sum\limits_{n}nx^{n}\left(\sum\limits_{m}y^{m}\right) = \sum\limits_{n}nx^{n}\left(\frac{1}{1-y}\right) = \left(\frac{1}{1-y}\right)\sum\limits_{n}nx^{n} = \left(\frac{1}{1-y}\right)\left(\frac{x}{(1 - x)^{2}}\right)$$
$$
\sum\limits_{n}\sum\limits_{m}mx^{n}y^{m} = \left(\frac{1}{1-x}\right)\sum\limits_{n} my^{m} = \left(\frac{1}{1-x}\right)\left(\frac{y}{(1 - y)^{2}}\right)
$$

$$\sum\limits_{n}\sum\limits_{m}a_{n,m}x^{n}y^{m} = \sum\limits_{n}\sum\limits_{m}nx^{n}y^{m} + \sum\limits_{n}\sum\limits_{m}mx^{n}y^{m} = \frac{y+x-2xy}{(1-y)^{2}(1-x)^{2}}$$

### Task 2
$$A(t) = \sum\limits_{n} \frac{a_{n}}{n!}t^{n}$$
$$\frac{d}{dt}\sum\limits_{n = 0} \frac{a_{n}}{n!}t^{n} = \sum\limits_{n = 1} \frac{a_{n}}{(n - 1)!}t^{n - 1}$$
$b_{n} = a_{n} * n$ - можем выбрать в качестве корня любой атом
$$B(t) = \sum\limits_{n = 0} \frac{na_{n}}{n!}t^{n} = \sum\limits_{n = 0} \frac{a_{n}}{(n - 1)!}t^{n} = t\frac{d}{dt}A(t) $$

### Task 3
Мультимножества размера 3 могут быть составлены тремя способами:
$$\{a, a, a\}, \{a, a, b\}, \{a, b, c\}\;\;\; a \neq b \neq c$$
$$\{a, a, a\} \leftrightarrow = \frac{A(t^{3})}{3}$$
$$\{a, a, b\} \leftrightarrow \frac{A(t^{2})}{2!} \frac{A(t)}{1!} =  \frac{A(t)A(t^{2})}{2}$$
$$\{a, b, c\} \leftrightarrow \frac{A(t)^{3}}{3!} = \frac{A(t)^{3}}{6}$$
$$\operatorname{MSet_{3}}(A) = \frac{A(t)^{3}}{6} + \frac{A(t)A(t^{2})}{2} + \frac{A(t^{3})}{3} = \frac{1}{6}\left(A(t)^{3}+ 3A(t)A(t^{2}) + 2A(t^{3})\right)$$

### Task 4
$S_{i} \in \{\{0\}, \{1\}, [0, 1]\}$, $|\{0\}| = |\{1\}| = 0$, $|[0, 1]| = 1$ - веса (влияние на размерность)
$$a_{nm} = {n \choose k} 2^{n-m} \text{  - колличество граней размерности m в n - мерном гиперкубе}$$
$$A(u, z) = \sum\limits_{n}\sum\limits_{m = 0}^{n}a_{nm}u^{m}z^{n} = \sum\limits_{n}\sum\limits_{m = 0}^{n}{n \choose k} 2^{n-m}u^{m}z^{n} = \sum\limits_{n}z^{n} \left(\sum\limits_{m = 0}^{n}{n \choose k} 2^{n-m}u^{m}\right)$$
$$\sum\limits_{m = 0}^{n}{n \choose k} 2^{n-m}u^{m} = \left[(\alpha+\beta)^{t} = \sum\limits_{k=0}^{t}{t\choose k}\alpha^{t-k}\beta^{k}, \;\; \alpha := 2, \beta := u, t := n, k:= m\right] = (2 + u)^{n}$$
$$A(u, z) = \sum\limits_{n}z^{n}(2 + u)^{n} = \frac{1}{1-(2+u)z}$$
