# 問21.4

$X$ を位相空間、$C(X)$ を $X$ 上で定義された実数値連続関数の集合とする。

$f,g\in C(X)$ とするとき、$f+g\in C(X)$ を示せ。

ここで

$$
(f+g)(x):=f(x)+g(x)
$$

と定義する。

---

任意に $a\in X$ を取る。

$(f+g)$ が $a$ で連続であることを示せばよい。

よって

$$
\forall U\in N((f+g)(a)),
\quad
(f+g)^{-1}(U)\in N(a)
$$

を示すこととする。

近傍の定義より、$U$ に対して

$$
\exists O\in\mathcal O_X,\quad
a\in O\subset (f+g)^{-1}(U)
$$

を示せば十分である。

---

$U\in N((f+g)(a))$ を任意に取る。

すると、ある正数 $\varepsilon>0$ が存在して

$$
B((f+g)(a),\varepsilon)\subset U
$$

となる。

ここで

$$
O_1=f^{-1}\!\left(B\!\left(f(a),\frac{\varepsilon}{2}\right)\right)
$$

とおくと、$f$ の連続性より $O_1$ は開集合であり、$a\in O_1$ である。

同様に

$$
O_2=g^{-1}\!\left(B\!\left(g(a),\frac{\varepsilon}{2}\right)\right)
$$

とおくと、$O_2$ は開集合であり、$a\in O_2$ である。

さて

$$
O=O_1\cap O_2
$$

とおく。当然 $a\in O$ である。

---

ここで

$$
O\subset (f+g)^{-1}(U)
$$

を示す。

$x\in O$ を任意に取る。

まず、$x\in O_1$ より

$$
\begin{aligned}
x\in O_1
&\iff
x\in
f^{-1}\!\left(B\!\left(f(a),\frac{\varepsilon}{2}\right)\right)\\
&\iff
f(x)\in
B\!\left(f(a),\frac{\varepsilon}{2}\right)\\
&\iff
|f(x)-f(a)|<\frac{\varepsilon}{2}.
\end{aligned}
$$

同様に、$x\in O_2$ より

$$
|g(x)-g(a)|<\frac{\varepsilon}{2}.
$$

続いて、三角不等式より

$$
\begin{aligned}
|(f+g)(x)-(f+g)(a)|
&=
|f(x)+g(x)-(f(a)+g(a))|\\
&=
|(f(x)-f(a))+(g(x)-g(a))|\\
&\le
|f(x)-f(a)|+|g(x)-g(a)|\\
&<
\frac{\varepsilon}{2}+\frac{\varepsilon}{2}
=
\varepsilon.
\end{aligned}
$$

したがって

$$
(f+g)(x)\in
B((f+g)(a),\varepsilon)
\subset U.
$$

よって

$$
(f+g)(x)\in U,
$$

すなわち

$$
x\in (f+g)^{-1}(U).
$$

$x\in O$ は任意であったから

$$
O\subset (f+g)^{-1}(U)
$$

が成り立つ。

したがって

$$
a\in O\subset (f+g)^{-1}(U)
$$

より

$$
(f+g)^{-1}(U)\in N(a).
$$

以上より、$(f+g)$ は $a$ で連続である。

$a$ は任意であったから

$$
f+g\in C(X).
\qquad\blacksquare
$$