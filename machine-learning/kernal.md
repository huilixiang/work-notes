# kernal
## 回顾“基”的概念
### 基本概念
在一个$$R^n$$的空间中， 我们可以使用n个独立向量的线性组合来表示任一向量。 这n个独立的向量可以被看到是一组”基“。 在一个$$R^n$$空间中， 有无穷组“基”。在这些基向量中， 每个向量与其它向量是正交的。例如：$$\{e_i\}_{i=1}^{n}$$ 是一组特殊的基向量， 除了第i个元素外， 其它元素都为0

### inner product
内积用来度量两个向量的相似性。 对于两个向量 x, y, 内积表示一个向量在另一个向量上的投影。 
$$ \left \langle X, Y \right \rangle = |X||Y|cos \theta $$
如果 $$X=(x_1, x_2,...,x_n), Y=(y_1, y_2, ...,y_n)$$ 则
$$ \left \langle X, Y \right \rangle = \sum_{i=1}^nx_iy_i $$

### function basis
一个函数f(x)可以看作是无限维的向量, 一个定义在区间[a, b]上的函数， 我们按区间$$\Delta x$$采样.  如果我们对函数f(x) 在以下点采样： $$ a, x_1, x_2,..., x_n, b $$, 则我们可以把函数f(x)转换成一个向量： $$(f(a), f(x_i), ..., f(x_n), f(b))^T$$. 当$$\Delta x \to 0$$, 这个向量会无限接近于f(x),  最后， 变成一个无穷维向量。

当把x换成一个向量的时间， 上面依然成立（不仅限于实数）。 f(x)用来表现函数在x处的值。 函数与向量是如此的相似，以至于我们可以像向量一样， 定义函数的内积。 对于两个函数：f , g, 按$$\Delta x$$采样， 则内积可以表示为：
$$\Large \left \langle f, g \right \rangle = lim_{\Delta x \to 0} \sum_{i}f(x_i)g(x_i) \Delta x = \int f(x)g(x)dx$$

向量有整数“维度”的概念， 不能有0.5维。 因此我们使用$$\Delta x$$ 来归一化。

### fourier series
让我们定义基函数： $$\{h_p\}_{p=-\infty}^{+\infty}$$.  p是整数。 
$$\Large h_p(x) = e^{\frac{i2\pi px}{T}}$$ , 定义在区间[0, T]上。 i是虚数。
我们来证明， 任意两个基函数是正交的：
$$\Large \left \langle h_p, h_q \right \rangle = \int_{0}^{T}h_p(x)\bar{h}_q(x) dx = \int_{0}^{T} e^{\frac{i2\pi px}{T}} e^{-\frac{i2\pi qx}{T}}dx = 0$$  导函数本质上是一个三角函数， 所以在一个周期内的积分为0。

复数的内积 $$ \left \langle u, v \right \rangle = \bar{v} * u , \bar{v}是v的共轭形式$$







