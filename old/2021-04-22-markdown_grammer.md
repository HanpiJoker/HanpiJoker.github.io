---
layout: post
author: HanpiJoker
title: Markdown Math Grammer
---

## Markdown 数学公式速记
### 公式插入
#### 行内或独行
1. 行内公式：将公式插入到本行内，符号：$公式内容$，如：$xyz$
2. 独行公式：将公式插入到新的一行内，并且居中，符号：$$公式内容$$，如：$$xyz$$

#### 上标、下标与组合
| 名称 | 符号 | 输入                  | 输出              |
|------|------|-----------------------|-------------------|
| 上标 | ^    | \$^4\$                | $x^4$             |
| 下标 | _    | \$x\_1\$              | $x_1$             |
| 组合 | {}   | \${T}\_{8}O{X}\_{2}\$ | ${T}_{8}O{X}_{2}$ |

#### 汉字、字体与格式
| 名称     | 符号                         | 输入                                                 | 输出                                               |
|----------|------------------------------|------------------------------------------------------|----------------------------------------------------|
| 汉字     | \mbox{}(有些引擎不需要)                      | \$V\_{\mbox{初始}}\$                                 | $V_{初始}$                                         |
| 字体     | \displaystyle                | \$\displaystyle \frac{x+y}{y+z}\$                    | $\displaystyle \frac{x+y}{y+z}$                    |
| 下划线   | \underline                   | \$\underline{x+y}\$                                  | $\underline{x+y}$                                  |
| 上大括号 | \overbrace{算式}             | \$\overbrace{a+b+c+d}^{2.0}\$                        | $\overbrace{a+b+c+d}^{2.0}$                        |
| 下大括号 | \underbrace{算式}            | \$a+\underbrace{b+c}_{1.0}+d\$                       | $a+\underbrace{b+c}_{1.0}+d$                       |
| 上位符号 | \stacrel{上位符号}{基位符号} | \$\vec{x}\stackrel{\mathrm{def}}{=}{x_1,\dots,x_n}\$ | $\vec{x}\stackrel{\mathrm{def}}{=}{x_1,\dots,x_n}$ |

#### 占位符
| 名称         | 符号   | 输入           | 输出         |
|--------------|--------|----------------|--------------|
| 两个quad空格 | \qquad | \$x \qquad y\$ | $x \qquad y$ |
| quad空格     | \quad  | \$x \quad y\$  | $x \quad y$  |
| 大空格       | \      | \$x \ y\$      | $x \ y$      |
| 中空格       | \:     | \$x \: y\$     | $x \: y$     |
| 小空格       | \,     | \$x \, y\$     | $x \, y$     |
| 没有空格     |        | \$xy\$         | $xy$         |
| 紧贴         | \!     | \$x \! y\$     | $x \! y$     |

#### 定界符与组合
| 名称       | 符号                                               | 输入                                                                   | 输出                                                                 |
|------------|----------------------------------------------------|------------------------------------------------------------------------|----------------------------------------------------------------------|
| 括号       | () \big(\big) \Big(\Big) \bigg(\bigg) \Bigg(\Bigg) | \$() \big(\big) \Big(\Big) \bigg(\bigg) \Bigg(\Bigg)\$                 | $（）\big(\big) \Big(\Big) \bigg(\bigg) \Bigg(\Bigg)$                |
| 中括号     | []                                                 | \$[x+y]\$                                                              | $[x+y]$                                                              |
| 大括号     | \{ \}                                              | \${x+y}\$                                                              | ${x+y}$                                                              |
| 自适应括号 | \left \right                                       | \$\left(x\right)\$; \$\left(x{yz}\right)\$                             | $\left(x\right)$; $\left(x{yz}\right)$                               |
| 组合公式   | {上位公式 \choose 下位公式}                        | \${n+1 \choose k}={n \choose k}+{n \choose k-1}\$                      | ${n+1 \choose k}={n \choose k}+{n \choose k-1}$                      |
| 组合公式   | {上位公式 \atop 下位公式}                          | \$\sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots\$ | $\sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots$ |

#### 四则运算
| 名称       | 符号                | 输入                  | 输出                                |
|------------|---------------------|-----------------------|-------------------------------------|
| 加法运算   | +                   | \$x+y=z\$             | $x+y=z$                             |
| 减法运算   | -                   | \$x-y=z\$             | $x-y=z$                             |
| 加减运算   | \pm                 | \$x \pm y=z\$         | $x \pm y=z$                         |
| 减加运算   | \mp                 | \$x \mp y=z\$         | $x \mp y=z$                         |
| 乘法运算   | \times              | \$x \times y=z\$      | $x \times y=z$                      |
| 点乘运算   | \cdot               | \$x \cdot y=z\$       | $x \cdot y=z$                       |
| 星乘运算   | \ast                | \$x \ast y=z\$        | $x \ast y=z$                        |
| 除法运算   | \div                | \$x \div y=z\$        | $x \div y=z$                        |
| 斜法运算   | /                   | \$x/y=z\$             | $x/y=z$                             |
| 分式表示   | \frac{分子}{分母}   | \$\frac{x+y}{y+z}\$   | $\frac{x+y}{y+z}$                   |
| 分式表示   | {分子} \voer {分母} | \${x+y} \over {y+z}\$ | ${x+y} \over {y+z}$                 |
| 绝对值表示 | \|                  | \$\| x+y \|\$         | \$\|x+y\|\$(表格中绝对值符号有冲突) |

#### 高级运算
| 名称         | 符号                    | 输入                                                         | 输出                                                       |
|--------------|-------------------------|--------------------------------------------------------------|------------------------------------------------------------|
| 开二次方运算 | \sqrt                   | \$\sqrt x\$                                                  | $\sqrt x$                                                  |
| 开方运算     | \sqrt[开方数]{被开方数} | \$\sqrt[3]{x+y}\$                                            | $\sqrt[3]{x+y}$                                            |
| 对数运算     | \log                    | \$\log(x)\$                                                  | $\log(x)$                                                  |
| 极限运算     | \lim                    | \$\lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}\$               | $\lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$               |
| 极限运算     | \displaystyle \lim      | \$\displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}\$ | $\displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$ |
| 求和运算     | \sum                    | \$\sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}\$               | $\sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}$               |
| 求和运算     | \displaystyle \sum      | \$\displaystyle \sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}\$ | $\displaystyle \sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}$ |
| 积分运算     | \int                    | \$\int^{\infty}_{0}{xdx}\$                                   | $\int^{\infty}_{0}{xdx}$                                   |

#### 逻辑运算
| 名称           | 符号     | 输入               | 输出             |
|----------------|----------|--------------------|------------------|
| 等于运算       | =        | \$x+y=z\$          | $x+y=z$          |
| 大于运算       | \>       | \$x+y>z\$          | $x+y>z$          |
| 小于运算       | \<       | \$x+y<z\$          | $x+y<z$          |
| 大于等于运算   | \geq     | \$x+y \geq z\$     | $x+y \geq z$     |
| 小于等于运算   | \leq     | \$x+y \leq z\$     | $x+y \leq z$     |
| 不等于运算     | \neq     | \$x+y \neq z\$     | $x+y \neq z$     |
| 不大于等于运算 | \ngeq    | \$x+y \ngeq z\$    | $x+y \ngeq z$    |
| 不大于等于运算 | \not\geq | \$x+y \not\geq z\$ | $x+y \not\geq z$ |
| 不小于等于运算 | \nleq    | \$x+y \nleq z\$    | $x+y \nleq z$    |
| 不小于等于运算 | \not\leq | \$x+y \not\leq z\$ | $x+y \not\leq z$ |
| 约等于运算     | \approx  | \$x+y \approx z\$  | $x+y \approx z$  |
| 恒定等于运算   | \equiv   | \$x+y \equiv z\$   | $x+y \equiv z$   |

#### 集合运算
| 名称         | 符号        | 输入                | 输出              |
|--------------|-------------|---------------------|-------------------|
| 属于运算     | \in         | \$x \in y\$         | $x \in y$         |
| 不属于运算   | \notin      | \$x \notin y\$      | $x \notin y$      |
| 不属于运算   | \not\in     | \$x \not\in y\$     | $x \not\in y$     |
| 子集运算     | \subset     | \$x \subset y\$     | $x \subset y$     |
| 子集运算     | \supset     | \$x \supset y\$     | $x \supset y$     |
| 真子集运算   | \subseteq   | \$x \subseteq y\$   | $x \subseteq y$   |
| 非真子集运算 | \subsetneq  | \$x \subsetneq y\$  | $x \subsetneq y$  |
| 真子集运算   | \supseteq   | \$x \supseteq y\$   | $x \supseteq y$   |
| 非真子集运算 | \supsetneq  | \$x \supsetneq y\$  | $x \supsetneq y$  |
| 非子集运算   | \not\subset | \$x \not\subset y\$ | $x \not\subset y$ |
| 非子集运算   | \not\supset | \$x \not\supset y\$ | $x \not\supset y$ |
| 并集运算     | \cup        | \$x \cup y\$        | $x \cup y$        |
| 交集运算     | \cap        | \$x \cap y\$        | $x \cap y$        |
| 差集运算     | \setminus   | \$x \setminus y\$   | $x \setminus y$   |
| 同或运算     | \bigodot    | \$x \bigodot y\$    | $x \bigodot y$    |
| 同与运算     | \bigotimes  | \$x \bigotimes y\$  | $x \bigotimes y$  |
| 实数集合     | \mathbb{R}  | \$\mathbb{R}\$      | $\mathbb{R}$      |
| 自然数集合   | \mathbb{Z}  | \$\mathbb{Z}\$      | $\mathbb{Z}$      |
| 空集         | \emptyset   | \$\emptyset\$       | $\emptyset$       |

#### 数学符号
| 名称             | 符号         | 输入                               | 输出                             |
|------------------|--------------|------------------------------------|----------------------------------|
| 无穷             | \infty       | \$\infty\$                         | $\infty$                         |
| 虚数             | \imath       | \$\imath\$                         | $\imath$                         |
| 虚数             | \jmath       | \$\jmath\$                         | $\jmath$                         |
| 数学符号         | \hat{a}      | \$\hat{a}\$                        | $\hat{a}$                        |
| 数学符号         | \check{a}    | \$\check{a}\$                      | $\check{a}$                      |
| 数学符号         | \breve{a}    | \$\breve{a}\$                      | $\breve{a}$                      |
| 数学符号         | \tilde{a}    | \$\tilde{a}\$                      | $\tilde{a}$                      |
| 数学符号         | \bar{a}      | \$\bar{a}\$                        | $\bar{a}$                        |
| 矢量符号         | \vec{a}      | \$\vec{a}\$                        | $\vec{a}$                        |
| 数学符号         | \acute{a}    | \$\acute{a}\$                      | $\acute{a}$                      |
| 数学符号         | \grave{a}    | \$\grave{a}\$                      | $\grave{a}$                      |
| 数学符号         | \mathring{a} | \$\mathring{a}\$                   | $\mathring{a}$                   |
| 一阶导数符号     | \dot{a}      | \$\dot{a}\$                        | $\dot{a}$                        |
| 二阶导数符号     | \ddot{a}     | \$\ddot{a}\$                       | $\ddot{a}$                       |
| 上箭头           | \uparrow     | \$\uparrow\$                       | $\uparrow$                       |
| 上箭头           | \Uparrow     | \$\Uparrow\$                       | $\Uparrow$                       |
| 下箭头           | \downarrow   | \$\downarrow\$                     | $\downarrow$                     |
| 下箭头           | \Downarrow   | \$\Downarrow\$                     | $\Downarrow$                     |
| 左箭头           | \leftarrow   | \$\leftarrow\$                     | $\leftarrow$                     |
| 左箭头           | \Leftarrow   | \$\Leftarrow\$                     | $\Leftarrow$                     |
| 右箭头           | \rightarrow  | \$\rightarrow$                     | $\rightarrow$                    |
| 右箭头           | \Rightarrow  | \$\Rightarrow\$                    | $\Rightarrow$                    |
| 底端对齐的省略号 | \ldots       | \$1,2,\ldots,n\$                   | $1,2,\ldots,n$                   |
| 中线对齐的省略号 | \cdots       | \$x_1^2 + x_2^2 + \cdots + x_n^2\$ | $x_1^2 + x_2^2 + \cdots + x_n^2$ |
| 竖直对齐的省略号 | \vdots       | \$\vdots\$                         | $\vdots$                         |
| 斜对齐的省略号   | \ddots       | \$\ddots\$                         | $\ddots$                         |

#### 希腊字母

| 字母 | 输入     | 输出       | 字母 | 实现     | 输出       |
|------|----------|------------|------|----------|------------|
| A    | A        | $A$        | α    | \alpha   | $\alpha$   |
| B    | B        | $B$        | β    | \beta    | $\beta$    |
| Γ    | \Gamma   | $\Gamma$   | γ    | \gamma   | $\gamma$   |
| Δ    | \Delta   | $\Delta$   | δ    | \delta   | $\delta$   |
| E    | E        | $E$        | ϵ    | \epsilon | $\epsilon$ |
| Z    | Z        | $Z$        | ζ    | \zeta    | $\zeta$    |
| H    | H        | $H$        | η    | \eta     | $\eta$     |
| Θ    | \Theta   | $\Theta$   | θ    | \theta   | $\theta$   |
| I    | I        | $I$        | ι    | \iota    | $\iota$    |
| K    | K        | $K$        | κ    | \kappa   | $\kappa$   |
| Λ    | \Lambda  | $\Lambda$  | λ    | \lambda  | $\lambda$  |
| M    | M        | $M$        | μ    | \mu      | $\mu$      |
| N    | N        | $N$        | ν    | \nu      | $\nu$      |
| Ξ    | \Xi      | $\Xi$      | ξ    | \xi      | $\xi$      |
| O    | O        | $O$        | ο    | \omicron | $\omicron$ |
| Π    | \Pi      | $\Pi$      | π    | \pi      | $\pi$      |
| P    | P        | $P$        | ρ    | \rho     | $\rho$     |
| Σ    | \Sigma   | $\Sigma$   | σ    | \sigma   | $\sigma$   |
| T    | T        | $T$        | τ    | \tau     | $\tau$     |
| Υ    | \Upsilon | $\Upsilon$ | υ    | \upsilon | $\upsilon$ |
| Φ    | \Phi     | $\Phi$     | ϕ    | \phi     | $\phi$     |
| X    | X        | $X$        | χ    | \chi     | $\chi$     |
| Ψ    | \Psi     | $\Psi$     | ψ    | \psi     | $\psi$     |
| Ω    | \Omega   | $\Omega$   | ω    | \omega   | $\omega$   |
