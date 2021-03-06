# **Shockley-James** 悖论

## by 刘成锴 518030910425

---

# 一、前言

为了解决牛顿力学和麦克斯韦电磁理论之间的矛盾，爱因斯坦提出了狭义相对论。基于对狭义相对论的正确理解，使许多表面上的悖论得到解决。那时候，讨论主要集中在电磁波的传播上。

现在，来解决一个不同类型的悖论。W. Schockley（物理诺奖得主、晶体管的发明人之一威廉·肖克利） 和 R. P. James于20世纪60年代末提出的一个简单的电荷系统。要理解这个系统中线动量的守恒性，需要作仔细的相对论分析。 如果一个点电荷处在一个磁环强度变化的磁体附近，这个电荷会感应电力的作用，但这个磁体不会受到表观的反作用力。 （假设这个过程非常慢，忽略任何电磁辐射以及任何由电磁波带走的动量）这样的话，我们似乎可以得到一个发射炮弹没有反冲（后坐力）的大炮。

在这个问题中，我们将对这个系统进行分析，并且通过探究发现，在相对论力学中，一个复合体系可以具有非零的机械动量，而仍然可以保持静止。

---

# 二、**Shockley-James** 悖论介绍

我们通过这样一个模型来理解Shockley-James悖论中的基本问题。

如图所示：

<img src="http://people.exeter.ac.uk/sh481/fig-1.png" alt="img" style="zoom:50%;" />

一个点电荷在一个静止的磁体（图中是一个电流环）的外部静止。电流环中的电流为 $j$ 。电荷的质量为$m$，电量为$q$，电荷的位置$x(t)$满足如下动力学方程：
$$
m \ddot{\boldsymbol{x}}=q[\boldsymbol{E}+\dot{\boldsymbol{x}} \times \boldsymbol{B}]=\mathbf{0}
$$
因为磁体不产生电场且电荷静止，磁体质心的位置$X(t)$满足如下方程

$$
M \ddot{\boldsymbol{X}}=\int[\rho \boldsymbol{E}+\boldsymbol{j} \times \boldsymbol{B}] d^{3} \boldsymbol{r}=\mathbf{0}
$$

其中，$\rho$是电荷密度，$M$是磁体的总质量。因为$\rho = 0$，且静止电荷$q$不产生磁场，所以以上等式成立。

以上便是系统的初态，电荷和磁体都处于静止状态。现在我们让 $j$ 逐渐减小至0（实际可行方法有很多，在此不具体阐述），该过程可能花费任意长的时间，并且忽略电流变化所产生的的任何辐射。由此会产生磁通量$\Phi$的变化。
$$
\oint \boldsymbol{E} \cdot d \boldsymbol{l}=-\frac{\partial \Phi}{\partial t}
$$
产生的感生电场会导致点电荷加速，如图所示：

<img src="http://people.exeter.ac.uk/sh481/fig-2.png" alt="img" style="zoom:50%;" />

然而，磁体并没有受到等大反向的力。有人可能会认为，由于电荷开始运动，会产生一个磁场，该磁场会推动磁体。确实有这样一个力，但是它是$\dot{\boldsymbol{x}} / c$ 小于电荷上的力的因数 ，并且取决于$m$ 。为了简化问题，我们考虑一个重电荷，它受到相同的力，但是与光速相比，其移动速度很小，因此产生的磁场可以忽略不计。

于是我们有一个悖论：在此之后，$j$ 减小到零，整个系统的质心从静止状态开始运动。在牛顿力学中，由于牛顿第三定律，封闭系统的质心以恒定速度运动。那么，电荷和磁体的相互作用不遵守牛顿第三定律了吗？

（以上为本人翻译，具体可以参考原版英文叙述 http://people.exeter.ac.uk/sh481/shockley-james.html）

---

# 三、构造模型进行分析

## （一）作用在点电荷上的冲量

为了方便计算，考虑一个半径为$r$，电流为$I_1$的圆形电流环，以及另一个更大的，半径$R \gg r$的圆形电流环，两个环共圆心，并且在同一平面上。并且，小电流环中的电流变化$i_{1}=d I_{1} / d t$。如图所示：

<img src="/Users/lck/Library/Application Support/typora-user-images/image-20191209110059333.png" alt="image-20191209110059333" style="zoom: 50%;" />



现在拿走大电流环，代之以在半径$R$处放一个带电质点$Q$，可以假设，在所关心的时间段内，该点电荷几乎不怎么动。如图所示：

<img src="/Users/lck/Library/Application Support/typora-user-images/image-20191209110128109.png" alt="image-20191209110128109" style="zoom:50%;" />

现在，我们可以尝试求出小电流环内电流从初值$I_{1}=I$变化到终值$I_{1}=0$过程中，点电荷受到的总的切向冲量的大小 $J$ 。

具体求解过程如下：

![物理解答1](/Users/lck/Desktop/其他课/大学物理/物理问题/电磁学问题(2)/物理解答1.png)

得到结果
$$
J = \frac{\mu_0r^2QI}{4R^2}
$$

---

## （二）电流环受到的反冲

为了方便计算，我们考虑一个与之前形状不同的电流环，来理解电流环受到的反冲力的来源。

![image-20191209171711353](/Users/lck/Library/Application Support/typora-user-images/image-20191209171711353.png)

如上图所示，我们考虑一个边长为$l$ 的正方形电流环。在此环距离为$R \gg l$ 处有一个点电荷$Q$。此环中有电流强度为$I$ 的电流流过（我们采用的电流环模型是一个不带电的绝缘空心管）。载流子可以沿着环自由运动。在环的转角处，载流子与管壁发生弹性碰撞而作直角转向。忽略载流子之间所有的相互作用。并且假设管子上同一横截面内所有载流子运动速度相同。假设环很重，其运动可以忽略。

现在我们来计算环内载流子的总的线动量大小 $p_{h i d}$ ，这个动量被称为“隐藏动量”（Reference : **Hidden Momentum** On Wikipedia）。

具体求解过程如下：

![物理解答2](/Users/lck/Desktop/其他课/大学物理/物理问题/电磁学问题(2)/物理解答2.png)

得到结果
$$
p_{h i d} = \frac{Q I l^2}{4 \pi \varepsilon_0 R^2 c^2}
$$

#### （*）解释

当电流停止时，此线动量将转移到环上，环获得一个冲量，该冲量与点电荷 $Q$ 受到的冲量大小相等，方向相反。这个冲量就是我们所要寻找的消失的反冲。（注意在初始状态下，电磁场中也有动量，这保证了整个系统的动量守恒）

---

## （三）验证计算结果

接下来我们引入磁矩$\mu=I S$来研究电流环，其中$I$ 为电流， $S$ 为环的面积。于是，我们将磁矩$\mu$代入（一）和（二）求得的结果$J$ 和 $p_{hid}$中。

#### （一）中$J$的结果

由于（一）中电流环的磁矩$\mu=\pi r^{2} I$，因此将$\mu$代入$J$后有
$$
J = \frac{\mu_{0} Q \mu}{4 \pi R^{2}}
$$

#### （二）中$p_{hid}$的结果

由于（二）中电流环的磁矩$$\mu=l^{2} I$$，因此将$\mu$代入$p_{hid}$后有
$$
p_{h i d}=\frac{Q \mu}{4 \pi \varepsilon_0R^{2} c^{2}}=\frac{\mu_{0} Q \mu}{4 \pi R^{2}}
$$


通过对比$J$ 和 $p_{hid}$，我们发现：
$$
J = p_{hid}
$$
即点电荷受到的冲量大小 $J$ 等于电流环内载流子的总线动量 $p_{hid}$ 的大小。（二）中的解释得到验证。

---

# 四、总结

本文介绍了Shockley-James悖论。

本问题采用了一个简单的模型，探究了Shockley-James悖论中关于 “如果一个点电荷处在一个磁环强度变化的磁体附近，这个电荷会感应电力的作用，但这个磁体不会受到表观的反作用力” 的问题。最终发现“在相对论力学中，一个复合体系可以具有非零的机械动量，而仍然可以保持静止”，并且得到一下具体结果：

>点电荷受到的冲量大小 $J$ 等于电流环内载流子的总线动量 $p_{hid}$ 的大小。
>
>当电流停止时，此线动量将转移到环上，环获得一个冲量，该冲量与点电荷 $Q$ 受到的冲量大小相等，方向相反。这个冲量就是我们所要寻找的消失的反冲。

由于本问题采用了一个简单的方便计算的模型，此模型或多或少存在一些疏漏之处，不能代表普遍情况。因此，我还通过查阅参考资料，了解到了更普遍的情况，经过我个人的理解，概括具体如下：

> **在更真实的模型中，电流环是一条导体电线，而点电荷 $Q$ 所产生的电场不能穿越进入于导体内。** 假设电流仍然是由电线中的载流子传导的。
>
> 考虑本问题中的情况，有以下性质：
>
> * 电流环的线性动量为0。
>
> 我个人对此理解如下：
>
> 由于点电荷 $Q$ 所产生的电场不能穿越进入导体内。因此不能像（二）中模型计算左边与右边的电势能之差$\Delta U$，这种 $\Delta U$ 为 0，因此电流环的线性动量为0。
>
> * 随着电流从 $I$ 变为0，由外部电荷在导线上感应出的表面电荷，将受到一个电场力。这样，电流环获得的冲量大小将与（二）中模型计算出来的一样。

由于本人水平有限，对Shockley-James悖论可能尚处于一知半解的状态，不能很好地阐述自己的问题和想法。并且由于本文参考资料主要为英语，在一些翻译上存在不恰当之处。烦请同学们对本文中的问题进行批评指正。

最后,欢迎大家讨论我的问题，提出⼀些意⻅和建议。 

谢谢！

---

# 参考资料

**1. Shockley-James Paradox**

http://people.exeter.ac.uk/sh481/shockley-james.html

**2. APHO Israel 2011 Theoretical Questions**

http://mpec.sc.mahidol.ac.th/apho10/sites/default/files/(1)%20shockley%20question.pdf

**3. Hidden momentum**

https://en.wikipedia.org/wiki/Hidden_momentum