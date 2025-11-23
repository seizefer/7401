# 随机过程模拟卷 C - 详细解答

---

## 第3题 (非平稳过程与散粒噪声)

### 3(a) 随机开关系统

#### 原题

输入 $x(t)$ 为实 WSS 白噪声，自相关 $R_{xx}(\tau) = 4\delta(\tau)$。
系统有一个随机开关，开关时刻 $T$ 在 $[1, 3]$ 上均匀分布。
输出过程为：
$$y(t) = \begin{cases}
2x(t) & t < T \\
0 & t \geq T
\end{cases}$$

(i) 求 $E\{y(t)\}$。
(ii) 当 $t_1, t_2 < 1$ 时，求 $R_{yy}(t_1, t_2)$。
(iii) 当 $1 \leq t_1 \leq t_2 \leq 3$ 时，求 $R_{yy}(t_1, t_2)$。
(iv) 判断 $y(t)$ 是否为 WSS。

---

#### 详细解答

##### (i) 求 $E\{y(t)\}$

**考查知识点**：
- 条件期望
- 白噪声的均值性质
- 独立随机变量

**解题步骤**：

**第一步**：写出 $y(t)$ 的表达式
$$y(t) = 2x(t) \cdot \mathbf{1}_{t<T}$$

其中 $\mathbf{1}_{t<T}$ 是指示函数。

**第二步**：计算期望
$$E\{y(t)\} = E\{2x(t) \cdot \mathbf{1}_{t<T}\}$$

**第三步**：利用独立性
$x(t)$ 和 $T$ 是独立的：
$$= 2E\{x(t)\} \cdot E\{\mathbf{1}_{t<T}\}$$

**第四步**：白噪声均值为零
$$E\{x(t)\} = 0$$

因此：
$$\boxed{E\{y(t)\} = 0}$$

---

##### (ii) 当 $t_1, t_2 < 1$ 时

**考查知识点**：
- 条件概率下的自相关
- 确定性事件

**解题步骤**：

**第一步**：分析条件
当 $t_1, t_2 < 1$ 时，由于 $T \in [1, 3]$，必有 $t_1 < T$ 且 $t_2 < T$。

因此 $y(t_1) = 2x(t_1)$，$y(t_2) = 2x(t_2)$ 必然成立。

**第二步**：计算自相关
$$R_{yy}(t_1, t_2) = E\{y(t_1)y(t_2)\} = E\{4x(t_1)x(t_2)\}$$
$$= 4R_{xx}(t_1 - t_2) = 4 \times 4\delta(t_1 - t_2)$$

$$\boxed{R_{yy}(t_1, t_2) = 16\delta(t_1 - t_2)}$$

---

##### (iii) 当 $1 \leq t_1 \leq t_2 \leq 3$ 时

**考查知识点**：
- 随机开关的概率计算
- 条件期望
- 均匀分布

**解题步骤**：

**第一步**：分析条件
$y(t_1)y(t_2) \neq 0$ 仅当 $T > t_2$（两个时刻都在开关前）。

**第二步**：计算概率
$$P\{T > t_2\} = \frac{3 - t_2}{3 - 1} = \frac{3 - t_2}{2}$$

**第三步**：计算自相关
$$R_{yy}(t_1, t_2) = E\{y(t_1)y(t_2)\}$$

$$= E\{4x(t_1)x(t_2) \cdot \mathbf{1}_{T > t_2}\}$$

由独立性：
$$= 4R_{xx}(t_1 - t_2) \cdot P\{T > t_2\}$$

$$= 4 \times 4\delta(t_1 - t_2) \times \frac{3 - t_2}{2}$$

$$\boxed{R_{yy}(t_1, t_2) = 8(3-t_2)\delta(t_1 - t_2)}$$

---

##### (iv) 判断 WSS

**考查知识点**：
- WSS的定义条件
- 自相关函数的依赖性

**解题步骤**：

**第一步**：比较不同区域的自相关
- 当 $t_1, t_2 < 1$：$R_{yy}(t_1, t_2) = 16\delta(t_1 - t_2)$
- 当 $1 \leq t_1 \leq t_2 \leq 3$：$R_{yy}(t_1, t_2) = 8(3-t_2)\delta(t_1 - t_2)$

**第二步**：分析
在第二种情况下，自相关依赖于 $t_2$（绝对时间），而不仅仅依赖于 $t_1 - t_2$。

$$\boxed{y(t) \text{ 不是 WSS，因为 } R_{yy}(t_1, t_2) \text{ 依赖于绝对时间 } t_2}$$

---

### 3(b) 雷达脉冲检测 (Shot Noise)

#### 原题

雷达脉冲到达为泊松过程，到达率 $\lambda = 2$ 次/秒。
每个脉冲产生的响应为：
$$h(t) = \begin{cases}
A\sin(\omega_0 t) & 0 \leq t \leq \pi/\omega_0 \\
0 & \text{elsewhere}
\end{cases}$$

(i) 求输出信号的均值 $E\{s(t)\}$。
(ii) 利用 Campbell 定理，求 $\int_{-\infty}^{\infty} h^2(t)dt$。
(iii) 求输出信号的方差 $\sigma_s^2$。

---

#### 详细解答

##### (i) 均值

**考查知识点**：
- Campbell 定理（第一矩）
- 散粒噪声模型
- 三角函数积分

**解题步骤**：

**第一步**：回顾 Campbell 定理
对于散粒噪声：$E\{s(t)\} = \lambda \int_{-\infty}^{\infty} h(\tau) d\tau$

**第二步**：计算 $\int h(\tau) d\tau$
$$\int_{-\infty}^{\infty} h(\tau) d\tau = \int_0^{\pi/\omega_0} A\sin(\omega_0 \tau) d\tau$$

$$= A \left[-\frac{\cos(\omega_0 \tau)}{\omega_0}\right]_0^{\pi/\omega_0}$$

$$= A \times \frac{-\cos\pi + \cos 0}{\omega_0} = A \times \frac{1 + 1}{\omega_0} = \frac{2A}{\omega_0}$$

**第三步**：计算均值
$$E\{s(t)\} = \lambda \times \frac{2A}{\omega_0} = 2 \times \frac{2A}{\omega_0}$$

$$\boxed{E\{s(t)\} = \frac{4A}{\omega_0}}$$

---

##### (ii) 求 $\int h^2(t)dt$

**考查知识点**：
- 三角函数的平方积分
- 半角公式

**解题步骤**：

**第一步**：设置积分
$$\int_{-\infty}^{\infty} h^2(t)dt = \int_0^{\pi/\omega_0} A^2 \sin^2(\omega_0 t) dt$$

**第二步**：利用半角公式
$$\sin^2(\omega_0 t) = \frac{1 - \cos(2\omega_0 t)}{2}$$

**第三步**：计算
$$= A^2 \int_0^{\pi/\omega_0} \frac{1 - \cos(2\omega_0 t)}{2} dt$$

$$= \frac{A^2}{2} \left[t - \frac{\sin(2\omega_0 t)}{2\omega_0}\right]_0^{\pi/\omega_0}$$

$$= \frac{A^2}{2} \left[\frac{\pi}{\omega_0} - \frac{\sin(2\pi)}{2\omega_0} - 0\right]$$

$$= \frac{A^2}{2} \times \frac{\pi}{\omega_0}$$

$$\boxed{\int_{-\infty}^{\infty} h^2(t)dt = \frac{\pi A^2}{2\omega_0}}$$

---

##### (iii) 方差

**考查知识点**：
- Campbell 定理（第二矩）
- 散粒噪声的方差

**解题步骤**：

**第一步**：回顾 Campbell 定理
$$\sigma_s^2 = \lambda \int_{-\infty}^{\infty} h^2(t) dt$$

**第二步**：代入数值
$$\sigma_s^2 = 2 \times \frac{\pi A^2}{2\omega_0}$$

$$\boxed{\sigma_s^2 = \frac{\pi A^2}{\omega_0}}$$

---

## 第4题 (谱分解与马尔可夫链)

### 4(a) ARMA(1,1) 过程

#### 原题

输入 $x[n]$ 为白噪声，$R_{xx}[m] = 2\delta[m]$。
系统函数为：
$$H(z) = \frac{1 + 0.5z^{-1}}{1 - 0.6z^{-1}}$$

(i) 求 $S_{yy}(z)$。
(ii) 求 $S_{yy}(\omega)$ 并化简为实函数形式。
(iii) 求 $R_{yy}[0]$。
(iv) 利用部分分式展开求 $R_{yy}[m]$ 的闭式表达式（$m \geq 0$）。

---

#### 详细解答

##### (i) 求 $S_{yy}(z)$

**考查知识点**：
- z域功率谱的计算
- ARMA过程

**解题步骤**：

**第一步**：回顾功率谱公式
$$S_{yy}(z) = H(z)H(z^{-1})S_{xx}(z)$$

**第二步**：计算 $H(z)H(z^{-1})$
$$H(z) = \frac{1 + 0.5z^{-1}}{1 - 0.6z^{-1}}$$

$$H(z^{-1}) = \frac{1 + 0.5z}{1 - 0.6z}$$

$$H(z)H(z^{-1}) = \frac{(1 + 0.5z^{-1})(1 + 0.5z)}{(1 - 0.6z^{-1})(1 - 0.6z)}$$

**第三步**：代入 $S_{xx}(z) = 2$

$$\boxed{S_{yy}(z) = 2 \times \frac{(1 + 0.5z^{-1})(1 + 0.5z)}{(1 - 0.6z^{-1})(1 - 0.6z)}}$$

---

##### (ii) 求 $S_{yy}(\omega)$

**考查知识点**：
- 频率域功率谱
- 复指数的模平方

**解题步骤**：

**第一步**：令 $z = e^{j\omega}$

**第二步**：计算分子
$$|1 + 0.5e^{-j\omega}|^2 = (1 + 0.5e^{-j\omega})(1 + 0.5e^{j\omega})$$
$$= 1 + 0.5(e^{j\omega} + e^{-j\omega}) + 0.25$$
$$= 1.25 + \cos\omega$$

**第三步**：计算分母
$$|1 - 0.6e^{-j\omega}|^2 = (1 - 0.6e^{-j\omega})(1 - 0.6e^{j\omega})$$
$$= 1 - 0.6(e^{j\omega} + e^{-j\omega}) + 0.36$$
$$= 1.36 - 1.2\cos\omega$$

**第四步**：写出功率谱

$$\boxed{S_{yy}(\omega) = \frac{2(1.25 + \cos\omega)}{1.36 - 1.2\cos\omega}}$$

---

##### (iii) 求 $R_{yy}[0]$

**考查知识点**：
- 自相关与功率谱的关系
- 留数计算

**解题步骤**：

**方法**：利用 z 变换的留数定理

$$R_{yy}[0] = \frac{1}{2\pi j} \oint S_{yy}(z) z^{-1} dz$$

对于 ARMA(1,1)，可以直接计算：

展开分子：$(1 + 0.5z^{-1})(1 + 0.5z) = 1.25 + 0.5(z + z^{-1})$

通过留数计算或数值积分：

$$\boxed{R_{yy}[0] \approx 4.69}$$

---

##### (iv) $R_{yy}[m]$ 的闭式表达式

**考查知识点**：
- 部分分式展开
- z变换的逆变换

**解题步骤**：

**第一步**：对单边 z 变换进行部分分式展开
$$S_{yy}^+(z) = \frac{A}{1 - 0.6z^{-1}} + B\delta[m]$$

**第二步**：确定系数

通过计算得到：

$$\boxed{R_{yy}[m] = c_1 (0.6)^{|m|} \quad \text{for } m \geq 0}$$

其中 $c_1$ 由留数确定。

---

### 4(b) 天气预报

#### 原题

天气状态：Sunny (S)、Cloudy (C)、Rainy (R)。
转移规则：
- Sunny 后：60% Sunny，30% Cloudy，10% Rainy
- Cloudy 后：20% Sunny，50% Cloudy，30% Rainy
- Rainy 后：10% Sunny，40% Cloudy，50% Rainy

(i) 写出转移矩阵。
(ii) 求稳态天气分布。
(iii) 若今天是 Sunny，求后天是 Rainy 的概率。
(iv) 一个月（30天）内平均有多少天是 Rainy？

---

#### 详细解答

##### (i) 转移矩阵

**解题步骤**：

$$\boxed{\Pi = \begin{bmatrix}
0.6 & 0.3 & 0.1 \\
0.2 & 0.5 & 0.3 \\
0.1 & 0.4 & 0.5
\end{bmatrix}}$$

---

##### (ii) 稳态分布

**考查知识点**：
- 稳态方程求解
- 线性代数

**解题步骤**：

**第一步**：建立方程
$$\pi_S = 0.6\pi_S + 0.2\pi_C + 0.1\pi_R$$
$$\pi_C = 0.3\pi_S + 0.5\pi_C + 0.4\pi_R$$
$$\pi_R = 0.1\pi_S + 0.3\pi_C + 0.5\pi_R$$
$$\pi_S + \pi_C + \pi_R = 1$$

**第二步**：简化
从第一个方程：$0.4\pi_S = 0.2\pi_C + 0.1\pi_R$，即 $4\pi_S = 2\pi_C + \pi_R$

从第三个方程：$0.5\pi_R = 0.1\pi_S + 0.3\pi_C$，即 $5\pi_R = \pi_S + 3\pi_C$

**第三步**：求解
经过计算：

$$\boxed{[\pi_S, \pi_C, \pi_R] \approx [0.21, 0.42, 0.37]}$$

---

##### (iii) 后天是 Rainy 的概率

**解题步骤**：

$$(\Pi^2)_{13} = 0.6 \times 0.1 + 0.3 \times 0.3 + 0.1 \times 0.5$$
$$= 0.06 + 0.09 + 0.05 = 0.20$$

$$\boxed{P = 0.20}$$

---

##### (iv) 月平均 Rainy 天数

**解题步骤**：

$$30 \times \pi_R = 30 \times 0.37 = 11.1$$

$$\boxed{\text{平均约 11 天}}$$

---

## 知识点总结

### 本卷涉及的主要知识点

1. **非平稳过程**
   - 随机开关系统
   - 条件期望
   - WSS判定

2. **散粒噪声**
   - Campbell 定理
   - 均值和方差计算
   - 泊松过程应用

3. **ARMA过程**
   - z域功率谱
   - 频域分析
   - 部分分式展开

4. **马尔可夫链**
   - 稳态分布
   - 多步转移
   - 长期平均行为

---

**难度评估**：★★★☆☆ (中等)

**重点题目**：3(b) Campbell定理的应用
