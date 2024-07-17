# 令和6年度 博士前期課程 入試解答
## 3. 離散構造

$ f_{n+1}(x) = x \lfloor f_n(x) \rfloor, f_0(x) = 1, x \in [0, \infty \rparen $ について。

$ \lfloor x \rfloor $ とはつまり小数部切り捨てのことである。


### (1)

シンプルに計算する。

$ f_1(1.5) = 1.5 \cdot \lfloor 1 \rfloor = 1.5 $

$ f_2(2.5) = 2.5 \cdot \lfloor f_1(2.5) \rfloor = 2.5 \cdot \lfloor 2.5 \cdot \lfloor 1 \rfloor \rfloor = 5 $

$ f_3(3.5) = 3.5 \cdot \lfloor 3.5 \cdot \lfloor 3.5 \rfloor \rfloor = 3.5 \cdot \lfloor 10.5 \rfloor = 35 $

### (2)

$ n = 1 $ において、$ f_1(x) = x $ であり、これは明らかに単射である。

よって真。

$ \forall x, y \in [0, \infty ), \; x \neq y \Rightarrow f(x) \neq f(y) $

### (3)

$ n = 2 $ において、 $ f_2(x) = x \cdot \lfloor x \rfloor $ である。ここで、 

$ f_2(x) = 0 \; (0 \le x \lt 1) $ 

$ f_2(x) \ge f_2(1) = 1 \; (1 \le x) $

であるから、たとえば $ f_2(x) = 0.5$ なる $x$ は存在しない。

全射の定義を満たさないので、命題は偽である。

### (4-1)

$ \forall k \in \mathbb{Z}_0 $ に対して、 $ n = m = 1, h = 2k $ と定めることで、$ f_n(h/2) = f_m(h/2) = f_1(2k/2) = k $ を満たすため、 $ (k, k) \in R $ である。

よって反射的。

### (4-2)

まず、$ (2,4) \in R $ である。 $ (n=1, m=2, h=4) $

また、$ (4,2) \in R $ である。 $ (n=2, m=1, h=4) $

これは反対象律の定義を満たさない。
