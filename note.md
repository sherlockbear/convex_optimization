# 凸性

## 凸集

### 开集，闭集，内部，边界

### 组合与包

- 线性包（子空间）：集合点的线性组合
- 仿射包：集合点的线性组合（系数和为1）。P集合的仿射包是包含P的最小仿射集
- 凸组合：特殊的线性组合，系数非负且和为一。凸组合是点集中点的加权平均值。
- 凸包：所有可能的凸组合的集合
- 锥组合：系数非负的线性组合
- 锥包：所有可能的锥组合的集合

### 凸集

定义：包含了任意两点间线段的集合：
$$
x_{1}, x_{2} \in C, \lambda \in[0,1] \Rightarrow \lambda x_{1}+(1-\lambda) x_{2} \in C
$$
凸集的维度由其仿射包的维度决定



## CH1 非线性优化

### 非线性优化的世界

#### 问题的一般形式

$$
\begin{array}{l}{\min f_{0}(x)} \\ {\text { s.t. } f_{j}(x) \& 0, \quad j=1 \ldots m} \\ {x \in Q}\end{array}
$$

其中
$$
\mathscr{F}=\left\{x \in Q | f_{j}(x) \leq 0, j=1 \ldots m\right\}
$$
称为问题的可行集

常见的类别包括：

- 有约束问题:$\mathscr{F} \nsubseteq \mathbb{R}^{n}$ .

- 无约束问题:$\mathscr{F}=\mathbb{R}^{n}​$.

- 平滑问题: all fj (·) are differentiable.

- 非平滑问题: there are several nondifferentiable components fk (·).

- 线性约束问题: 约束函数是仿射的:

  $$
  f_{j}(x)=\sum_{i=1}^{n} a_{j}^{(i)} x^{(i)}+b_{j} \equiv\left\langle a_{j}, x\right\rangle+ b_{j}, j=1 \ldots m
  $$

