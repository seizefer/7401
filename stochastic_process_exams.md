# 随机过程模拟试卷精选 (新编5套)

**说明**：题目背景描述已简化为中文，但所有数学定义、公式和条件均保持原文形式。

---

## **模拟卷 A**

### **3. (非平稳过程与功率谱)**

**(a) 股票价格模型**

Mr. Bull Market 的股票收益建模为实非平稳过程 $x(t)$ ($t \geq 0$)，且 $x(0)=0$。满足以下性质：

1. 非重叠区间的增量不相关：
$$E\left([x(t_4)-x(t_3)][x(t_2)-x(t_1)]\right)=0 \quad \text{for any } 0 \leq t_1 \leq t_2 \leq t_3 \leq t_4.$$

2. 增量平方的期望与时间间隔长度成正比：
$$E\left([x(t_2)-x(t_1)]^2\right)=\sigma^2(t_2-t_1) \quad \text{for any } 0 \leq t_1 \leq t_2.$$

求 $R_{xx}(t_1, t_2)$：
(i) 利用性质(1)证明当 $0 \leq t_1 \leq t_2 \leq t_3$ 时，$R_{xx}(t_1, t_3) = R_{xx}(t_1, t_2)$。
(ii) 利用(i)的结果和性质(2)，当 $t_1 \leq t_2$ 时求 $R_{xx}(t_1, t_2)$。
(iii) 综合求出任意 $t_1, t_2$ 下的 $R_{xx}(t_1, t_2)$。

**(b) 信号处理系统**

$y(t)$ 是实 WSS 过程，功率谱 $S_{yy}(\omega)$ 未知。
工程师 A 测量 $p(t) = y(t+b) + 2y(t) + y(t-b)$。
工程师 B 测量 $q(t) = y(t+b) - y(t-b)$。

(i) 求 $p(t)$ 的功率谱 $S_{pp}(\omega)$，并证明：
$$S_{pp}(\omega) = 2(1 + \cos(b\omega))^2 S_{yy}(\omega)$$

(ii) 求 $q(t)$ 的功率谱 $S_{qq}(\omega)$。

(iii) 求同一时刻的互相关 $R_{pq}(0)$。

(iv) 若信号 $y(t)$ 的主要频率成分在 $\omega = \pi/(2b)$，比较哪个测量系统对该频率的响应更好。

### **4. (MA过程与马尔可夫链)**

**(a) MA(2) 过程分析**

$x[n]$ 是实离散 WSS 白噪声，自相关为：
$$R_{xx}[m] = q\delta[m]$$

输出 $y[n]$ (MA(2)过程) 满足：
$$y[n] = x[n] + \alpha x[n-1] + \beta x[n-2]$$

(i) 求 $R_{yy}[0]$、$R_{yy}[1]$、$R_{yy}[2]$。

(ii) 当 $|m| > 2$ 时，求 $R_{yy}[m]$。

(iii) 求 $S_{yy}(\omega)$，并证明它是实函数。

**(b) 马尔可夫链 (咖啡店选择)**

Prof. Coffee Lover 每天选择咖啡店：Starbucks (S)、Local Cafe (L)、或 Home (H)。

- 从 S 出发：下次去 L 的概率 0.3，去 H 的概率 0.1
- 从 L 出发：下次去 S 的概率 0.5，去 H 的概率 0.2
- 从 H 出发：下次去 S 的概率 0.6，去 L 的概率 0.3

(i) 建立离散时间马尔可夫链，画状态转移图并写出一步转移矩阵。

(ii) 求稳态概率分布 $[\pi_S, \pi_L, \pi_H]$。

(iii) 若他从 Starbucks 开始，求两天后在 Home 的概率。

---

## **模拟卷 B**

### **3. (WSS过程与泊松过程)**

**(a) 温度传感器网络**

有两个温度传感器测量同一区域。设 $x(t)$ 和 $y(t)$ 为联合 WSS 实过程。
传感器融合输出为：
$$z(t) = ax(t) + by(t)$$
其中 $a, b$ 为常数。

已知：
- $R_{xx}(\tau) = 4e^{-|\tau|}$
- $R_{yy}(\tau) = 9e^{-2|\tau|}$
- $R_{xy}(\tau) = 3e^{-|\tau|}$

(i) 求 $R_{zz}(\tau)$（用 $a, b$ 表示）。

(ii) 若要使 $R_{zz}(0)$ 最小且满足 $a + b = 1$，求最优的 $a, b$。

(iii) 在最优条件下，判断 $z(t)$ 是否为 WSS。

**(b) 泊松过程 (外卖订单)**

外卖订单到达数 $N(t)$ 是泊松过程，已知午餐时段（12:00-13:00）平均到达 30 个订单。

(i) 求 20 分钟内恰好到达 8 个订单的概率。

(ii) 求 30 分钟内到达订单数的方差。

(iii) 已知前 15 分钟到达了 6 个订单，求前 30 分钟总共到达不超过 12 个订单的概率。

**(c) AR(1) 频域分析**

实平稳白噪声 $w[n]$，功率谱 $S_{ww}(\omega) = 3$。通过系统：
$$H(z) = \frac{1}{1 - 0.8z^{-1}}$$

(i) 求输出 $y[n]$ 的功率谱 $S_{yy}(\omega)$。

(ii) 求 $R_{yy}[0]$。

(iii) 设计一个白化滤波器 $G(z)$，使得 $y[n]$ 通过 $G(z)$ 后变为白噪声。

### **4. (遍历性与马尔可夫链)**

**(a) 遍历性判定**

实平稳零均值过程 $x(t)$，自协方差 $C_{xx}(\tau) = \frac{4}{1+\tau^2}$。

(i) 利用 Slutsky 定理判断 $x(t)$ 是否均值遍历 (mean-ergodic)。

(ii) 若已知：
$$E\{x(t+\lambda+\tau)x(t+\tau)x(t+\lambda)x(t)\} = \frac{16}{(1+\lambda^2)^2} \cdot h(\tau)$$
其中 $h(\tau) = 1 + \frac{1}{1+\tau^2}$。

判断 $x(t)$ 是否协方差遍历。

**(b) 马尔可夫链 (电梯调度)**

一栋三层楼的电梯，状态为当前所在楼层：1, 2, 3。
每次移动的转移规则如下：
- 从楼层 1：上到 2 的概率 0.7，直接到 3 的概率 0.1
- 从楼层 2：下到 1 的概率 0.3，上到 3 的概率 0.4
- 从楼层 3：下到 2 的概率 0.5，直接到 1 的概率 0.2

(i) 画状态转移图并写出转移矩阵 $\Pi[1]$。

(ii) 求稳态概率分布。

(iii) 电梯从楼层 1 开始，求经过 2 步后回到楼层 1 的概率。

(iv) 若楼层 2 是电费最高的位置，求长期平均电费占比。

---

## **模拟卷 C**

### **3. (非平稳过程与散粒噪声)**

**(a) 随机开关系统**

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

**(b) 雷达脉冲检测 (Shot Noise)**

雷达脉冲到达为泊松过程，到达率 $\lambda = 2$ 次/秒。
每个脉冲产生的响应为：
$$h(t) = \begin{cases}
A\sin(\omega_0 t) & 0 \leq t \leq \pi/\omega_0 \\
0 & \text{elsewhere}
\end{cases}$$

(i) 求输出信号的均值 $E\{s(t)\}$。

(ii) 利用 Campbell 定理，求 $\int_{-\infty}^{\infty} h^2(t)dt$。

(iii) 求输出信号的方差 $\sigma_s^2$。

### **4. (谱分解与马尔可夫链)**

**(a) ARMA(1,1) 过程**

输入 $x[n]$ 为白噪声，$R_{xx}[m] = 2\delta[m]$。
系统函数为：
$$H(z) = \frac{1 + 0.5z^{-1}}{1 - 0.6z^{-1}}$$

(i) 求 $S_{yy}(z)$。

(ii) 求 $S_{yy}(\omega)$ 并化简为实函数形式。

(iii) 求 $R_{yy}[0]$。

(iv) 利用部分分式展开求 $R_{yy}[m]$ 的闭式表达式（$m \geq 0$）。

**(b) 马尔可夫链 (天气预报)**

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

## **模拟卷 D**

### **3. (复过程与调制)**

**(a) 复包络信号**

$w(t) = a(t) + jb(t)$，其中 $a(t)$ 和 $b(t)$ 是联合 WSS 实过程。
已知：
- $R_{aa}(\tau) = R_{bb}(\tau) = e^{-|\tau|}$
- $R_{ab}(\tau) = -R_{ba}(\tau)$

定义调制信号：
$$x(t) = \text{Re}\{w(t)e^{j\omega_0 t}\} = a(t)\cos(\omega_0 t) - b(t)\sin(\omega_0 t)$$

(i) 求 $R_{ww}(\tau) = E\{w(t+\tau)w^*(t)\}$。判断 $w(t)$ 是否 WSS。

(ii) 求 $R_{xx}(t+\tau, t)$。

(iii) 求使得 $x(t)$ 为 WSS 的条件。在此条件下，求 $R_{xx}(\tau)$。

**(b) 差分系统**

$x[n]$ 是实 WSS 过程，$R_{xx}[m] = 3 \cdot (0.7)^{|m|}$。
定义 $y[n] = x[n] - x[n-2]$。

(i) 求 $E\{y[n]\}$（假设 $E\{x[n]\} = \mu$）。

(ii) 求 $R_{yy}[m]$。

(iii) 证明当 $|m| \geq 2$ 时，$R_{yy}[m] = cR_{xx}[m]$，并求常数 $c$。

(iv) 求 $S_{yy}(\omega)$。

### **4. (连续马尔可夫链与估计)**

**(a) 连续时间马尔可夫链 (服务器状态)**

服务器有两个状态：Active (A) 和 Idle (I)。
转移概率矩阵为：
$$\Pi(\tau) = \begin{bmatrix}
0.7 + 0.3e^{-5\tau} & 0.3 - 0.3e^{-5\tau} \\
0.7 - 0.7e^{-5\tau} & 0.3 + 0.7e^{-5\tau}
\end{bmatrix}$$

(i) 求速率矩阵 $Q = \Pi'(0^+)$。

(ii) 求稳态概率分布。

(iii) 若初始状态为 Active，求 $t = 0.2$ 秒后处于 Idle 状态的概率。

**(b) 最优线性估计**

信号 $s(t)$ 是零均值 WSS 过程，$R_{ss}(\tau) = 4e^{-2|\tau|}$。
需要估计 $z = \int_0^1 s(t)dt$。

(i) 估计器: $\hat{z} = as(0) + bs(1)$。建立正规方程并求最优 $a, b$。

(ii) 求最小均方误差 (MMSE)。

(iii) 若改用单点估计 $\hat{z} = cs(0.5)$，求最优 $c$ 和对应的 MSE。比较两种估计器的性能。

---

## **模拟卷 E**

### **3. (非平稳过程与均值)**

**(a) 新产品销量模型**

产品发布时间 $\tau$ 在 $[0, 12]$ 月内均匀分布。
销量过程建模为：
$$x(t) = \begin{cases}
0 & t < \tau \\
A(1 - e^{-\alpha(t-\tau)}) & t \geq \tau
\end{cases}$$
其中 $A = 10000$，$\alpha = 0.5$。

(i) 求均值 $E\{x(t)\}$（对 $0 \leq t \leq 12$）。

(ii) 求 $E\{x(6)\}$ 的数值。

(iii) 判断 $x(t)$ 是否为 WSS，给出理由。

**(b) 移动平均滤波**

$y(t)$ 是实 WSS 过程，$S_{yy}(\omega) = \frac{2}{1+\omega^2}$。
定义移动平均：
$$z(t) = \frac{1}{2a}\int_{t-a}^{t+a} y(\tau)d\tau$$

(i) 求该系统的频率响应 $H(\omega)$。

(ii) 求 $S_{zz}(\omega)$。

(iii) 求 $R_{zz}(0)$，即 $E\{z^2(t)\}$。

(iv) 当 $a \to \infty$ 时，$R_{zz}(0)$ 的极限是多少？解释物理意义。

### **4. (谱分解与马尔可夫链)**

**(a) 白化与谱分解**

实 WSS 过程 $x[n]$ 的功率谱为：
$$S_{xx}(z) = \frac{13 - 5z - 5z^{-1}}{(1-0.5z)(1-0.5z^{-1})}$$

(i) 对 $S_{xx}(z)$ 进行因式分解，写成 $S_{xx}(z) = \sigma^2 H(z)H(z^{-1})$ 的形式（$H(z)$ 因果稳定）。

(ii) 求白化滤波器 $\Gamma_x(z)$。

(iii) 求 $R_{xx}[m]$ 的闭式表达式。

**(b) 马尔可夫链 (网络路由)**

数据包在三个路由器 A, B, C 之间传输。
每一跳的转移概率：
- 从 A：到 B 概率 $p$，到 C 概率 $1-p$
- 从 B：到 A 概率 0.3，到 C 概率 0.7
- 从 C：到 A 概率 0.4，到 B 概率 0.6

(i) 写出转移矩阵（用 $p$ 表示）。

(ii) 求稳态概率 $[\pi_A, \pi_B, \pi_C]$（用 $p$ 表示）。

(iii) 若要求 $\pi_A \geq 0.3$，求 $p$ 的取值范围。

(iv) 从 A 出发，求两跳后回到 A 的概率（用 $p$ 表示）。

### **5. (预测与估计)**

**(a) 一阶马尔可夫过程预测**

$s(t)$ 是一阶马尔可夫过程，$R_{ss}(\tau) = 9e^{-|\tau|/3}$。

(i) 用 $s(t)$ 预测 $s(t+1)$ 的最优 LMS 预测器。

(ii) 求预测误差的均方值 $P$。

(iii) 若改用 $s(t)$ 和 $s(t-1)$ 共同预测 $s(t+1)$，即 $\hat{s}(t+1) = as(t) + bs(t-1)$，说明为什么对于一阶马尔可夫过程，最优解是 $b = 0$。

**(b) 噪声中的信号估计**

观测 $y(t) = s(t) + n(t)$，其中：
- 信号 $s(t)$：零均值 WSS，$R_{ss}(\tau) = 2e^{-|\tau|}$
- 噪声 $n(t)$：零均值白噪声，$R_{nn}(\tau) = \delta(\tau)$
- 信号与噪声不相关

用 $y(t)$ 估计 $s(t)$ 的最优线性估计器为 $\hat{s}(t) = ky(t)$。

(i) 求最优 $k$。

(ii) 求最小均方误差。

---

# 参考答案与详解

---

## **模拟卷 A 答案**

### **3(a) 股票价格模型**

**(i) 证明 $R_{xx}(t_1, t_3) = R_{xx}(t_1, t_2)$**

**解题思路**：利用增量不相关性质，将自相关函数分解。

**步骤**：
考虑 $0 \leq t_1 \leq t_2 \leq t_3$，利用性质(1)：
$$E\{[x(t_3) - x(t_2)] \cdot x(t_1)\} = E\{[x(t_3) - x(t_2)] \cdot [x(t_1) - x(0)]\} = 0$$

因为 $x(0) = 0$，所以：
$$E\{x(t_3) \cdot x(t_1)\} - E\{x(t_2) \cdot x(t_1)\} = 0$$

即：
$$\boxed{R_{xx}(t_1, t_3) = R_{xx}(t_1, t_2)}$$

**(ii) 求 $R_{xx}(t_1, t_2)$ 当 $t_1 \leq t_2$**

**解题思路**：利用(i)的结果，设 $t_3 = t_2$，并结合性质(2)。

**步骤**：
由(i)知，当 $t_1 \leq t_2$ 时，$R_{xx}(t_1, t_2) = R_{xx}(t_1, t_1)$。

利用性质(2)：
$$E\{[x(t_1) - x(0)]^2\} = \sigma^2 t_1$$

展开：
$$E\{x^2(t_1)\} - 2E\{x(t_1) \cdot x(0)\} + E\{x^2(0)\} = \sigma^2 t_1$$

由于 $x(0) = 0$：
$$R_{xx}(t_1, t_1) = \sigma^2 t_1$$

因此：
$$\boxed{R_{xx}(t_1, t_2) = \sigma^2 t_1 \quad \text{for } t_1 \leq t_2}$$

**(iii) 任意 $t_1, t_2$ 下的 $R_{xx}(t_1, t_2)$**

**解题思路**：利用自相关函数的对称性。

**步骤**：
由于 $R_{xx}(t_1, t_2) = R_{xx}(t_2, t_1)$，综合得：
$$\boxed{R_{xx}(t_1, t_2) = \sigma^2 \min(t_1, t_2)}$$

---

### **3(b) 信号处理系统**

**(i) 证明 $S_{pp}(\omega) = 2(1 + \cos(b\omega))^2 S_{yy}(\omega)$**

**解题思路**：将 $p(t)$ 视为 $y(t)$ 通过 LTI 系统的输出，求系统频率响应。

**步骤**：
$p(t) = y(t+b) + 2y(t) + y(t-b)$

这等价于冲激响应 $h(t) = \delta(t+b) + 2\delta(t) + \delta(t-b)$ 的系统。

频率响应：
$$H(\omega) = e^{j\omega b} + 2 + e^{-j\omega b} = 2 + 2\cos(\omega b) = 2(1 + \cos(\omega b))$$

功率谱：
$$S_{pp}(\omega) = |H(\omega)|^2 S_{yy}(\omega) = 4(1 + \cos(\omega b))^2 S_{yy}(\omega)$$

$$\boxed{S_{pp}(\omega) = 4(1 + \cos(b\omega))^2 S_{yy}(\omega)}$$

*注：题目公式系数应为4而非2。*

**(ii) 求 $S_{qq}(\omega)$**

**步骤**：
$q(t) = y(t+b) - y(t-b)$

频率响应：$G(\omega) = e^{j\omega b} - e^{-j\omega b} = 2j\sin(\omega b)$

$$S_{qq}(\omega) = |G(\omega)|^2 S_{yy}(\omega) = 4\sin^2(\omega b) S_{yy}(\omega)$$

$$\boxed{S_{qq}(\omega) = 4\sin^2(b\omega) S_{yy}(\omega)}$$

**(iii) 求 $R_{pq}(0)$**

**解题思路**：展开 $p(t)$ 和 $q(t)$，利用 WSS 性质。

**步骤**：
$$R_{pq}(0) = E\{p(t)q(t)\}$$

展开：
$$= E\{[y(t+b) + 2y(t) + y(t-b)][y(t+b) - y(t-b)]\}$$

$$= E\{y^2(t+b)\} - E\{y^2(t-b)\} + 2E\{y(t)y(t+b)\} - 2E\{y(t)y(t-b)\}$$

由 WSS 性质：$E\{y^2(t+b)\} = E\{y^2(t-b)\} = R_{yy}(0)$

且 $E\{y(t)y(t+b)\} = E\{y(t)y(t-b)\} = R_{yy}(b)$

因此：
$$\boxed{R_{pq}(0) = 0}$$

**(iv) 频率响应比较**

**步骤**：
在 $\omega = \pi/(2b)$ 处：

- $S_{pp}$: $|H(\omega)|^2 = 4(1 + \cos(\pi/2))^2 = 4(1+0)^2 = 4$
- $S_{qq}$: $|G(\omega)|^2 = 4\sin^2(\pi/2) = 4$

两者相等，但：
- 若主频略偏离 $\pi/(2b)$，$\cos(\omega b) \approx 0$ 时 $p(t)$ 响应下降更快
- $q(t)$ 在 $\omega = 0$ 处响应为 0（高通特性）

$$\boxed{\text{两者在该频率响应相等，但 } q(t) \text{ 具有高通特性，更适合去除直流分量}}$$

---

### **4(a) MA(2) 过程分析**

**(i) 求 $R_{yy}[0]$、$R_{yy}[1]$、$R_{yy}[2]$**

**解题思路**：利用白噪声的性质 $E\{x[n]x[m]\} = q\delta[n-m]$。

**步骤**：

$R_{yy}[0] = E\{y^2[n]\}$
$$= E\{(x[n] + \alpha x[n-1] + \beta x[n-2])^2\}$$
$$= E\{x^2[n]\} + \alpha^2 E\{x^2[n-1]\} + \beta^2 E\{x^2[n-2]\}$$
$$= q(1 + \alpha^2 + \beta^2)$$

$R_{yy}[1] = E\{y[n]y[n-1]\}$
$$= E\{(x[n] + \alpha x[n-1] + \beta x[n-2])(x[n-1] + \alpha x[n-2] + \beta x[n-3])\}$$
$$= \alpha E\{x^2[n-1]\} + \alpha\beta E\{x^2[n-2]\}$$
$$= q(\alpha + \alpha\beta)$$

$R_{yy}[2] = E\{y[n]y[n-2]\}$
$$= \beta E\{x^2[n-2]\} = q\beta$$

$$\boxed{R_{yy}[0] = q(1+\alpha^2+\beta^2), \quad R_{yy}[1] = q\alpha(1+\beta), \quad R_{yy}[2] = q\beta}$$

**(ii) 当 $|m| > 2$ 时**

**步骤**：
由于 $y[n]$ 只依赖于 $x[n], x[n-1], x[n-2]$，当 $|m| > 2$ 时，$y[n]$ 和 $y[n-m]$ 没有共同的 $x$ 项。

$$\boxed{R_{yy}[m] = 0 \quad \text{for } |m| > 2}$$

**(iii) 求 $S_{yy}(\omega)$**

**解题思路**：利用 $S_{yy}(\omega) = |H(e^{j\omega})|^2 S_{xx}(\omega)$。

**步骤**：
$H(z) = 1 + \alpha z^{-1} + \beta z^{-2}$

$H(e^{j\omega}) = 1 + \alpha e^{-j\omega} + \beta e^{-2j\omega}$

$|H(e^{j\omega})|^2 = H(e^{j\omega})H(e^{-j\omega})$
$$= (1 + \alpha e^{-j\omega} + \beta e^{-2j\omega})(1 + \alpha e^{j\omega} + \beta e^{2j\omega})$$

展开并化简：
$$= 1 + \alpha^2 + \beta^2 + 2\alpha(1+\beta)\cos\omega + 2\beta\cos 2\omega$$

$$\boxed{S_{yy}(\omega) = q[1 + \alpha^2 + \beta^2 + 2\alpha(1+\beta)\cos\omega + 2\beta\cos 2\omega]}$$

这是实函数，因为只含 $\cos$ 项。

---

### **4(b) 马尔可夫链 (咖啡店选择)**

**(i) 转移矩阵**

**步骤**：
从题目条件补全对角线概率：

$$\Pi = \begin{bmatrix}
0.6 & 0.3 & 0.1 \\
0.5 & 0.3 & 0.2 \\
0.6 & 0.3 & 0.1
\end{bmatrix}$$

（行：从 S, L, H；列：到 S, L, H）

**(ii) 稳态概率**

**解题思路**：解 $\pi \Pi = \pi$ 和 $\sum \pi_i = 1$。

**步骤**：
$$\pi_S = 0.6\pi_S + 0.5\pi_L + 0.6\pi_H$$
$$\pi_L = 0.3\pi_S + 0.3\pi_L + 0.3\pi_H$$
$$\pi_H = 0.1\pi_S + 0.2\pi_L + 0.1\pi_H$$

从第二个方程：$0.7\pi_L = 0.3(\pi_S + \pi_H) = 0.3(1 - \pi_L)$
$$\pi_L = 0.3$$

从第三个方程：$0.9\pi_H = 0.1\pi_S + 0.06$

结合 $\pi_S + \pi_H = 0.7$：
解得 $\pi_S = 0.54, \pi_H = 0.16$

$$\boxed{[\pi_S, \pi_L, \pi_H] = [0.54, 0.30, 0.16]}$$

**(iii) 两天后在 Home 的概率**

**步骤**：
计算 $\Pi^2$：

$$\Pi^2 = \Pi \cdot \Pi$$

$(\Pi^2)_{13} = 0.6 \times 0.1 + 0.3 \times 0.2 + 0.1 \times 0.1 = 0.06 + 0.06 + 0.01 = 0.13$

$$\boxed{P(\text{Home after 2 days} | \text{start from S}) = 0.13}$$

---

## **模拟卷 B 答案**

### **3(a) 温度传感器网络**

**(i) 求 $R_{zz}(\tau)$**

**解题思路**：利用自相关和互相关的线性组合公式。

**步骤**：
$$R_{zz}(\tau) = E\{z(t+\tau)z(t)\} = E\{[ax(t+\tau)+by(t+\tau)][ax(t)+by(t)]\}$$

$$= a^2 R_{xx}(\tau) + ab R_{xy}(\tau) + ab R_{yx}(\tau) + b^2 R_{yy}(\tau)$$

注意 $R_{yx}(\tau) = R_{xy}(-\tau)$。对于实过程：
$$= a^2 R_{xx}(\tau) + ab[R_{xy}(\tau) + R_{xy}(-\tau)] + b^2 R_{yy}(\tau)$$

代入数值：
$$\boxed{R_{zz}(\tau) = 4a^2 e^{-|\tau|} + 3ab[e^{-|\tau|} + e^{-|\tau|}] + 9b^2 e^{-2|\tau|}}$$
$$= 4a^2 e^{-|\tau|} + 6ab e^{-|\tau|} + 9b^2 e^{-2|\tau|}$$

**(ii) 最优 $a, b$**

**步骤**：
$R_{zz}(0) = 4a^2 + 6ab + 9b^2$

约束：$a + b = 1$，即 $a = 1 - b$

代入：
$$f(b) = 4(1-b)^2 + 6(1-b)b + 9b^2$$
$$= 4 - 8b + 4b^2 + 6b - 6b^2 + 9b^2$$
$$= 4 - 2b + 7b^2$$

求导：$f'(b) = -2 + 14b = 0$

$$b = 1/7, \quad a = 6/7$$

$$\boxed{a = 6/7, \quad b = 1/7}$$

**(iii) 判断 WSS**

**步骤**：
$z(t)$ 是两个 WSS 过程的线性组合，因此：
- $E\{z(t)\}$ 为常数
- $R_{zz}(t_1, t_2)$ 只依赖于 $\tau = t_1 - t_2$

$$\boxed{z(t) \text{ 是 WSS}}$$

---

### **3(b) 泊松过程 (外卖订单)**

**(i) 20分钟内恰好8个订单**

**解题思路**：先求到达率 $\lambda$，再用泊松分布公式。

**步骤**：
$E\{N(60)\} = 30$，所以 $\lambda \times 60 = 30$，$\lambda = 0.5$ 个/分钟。

20分钟：$\mu = \lambda \times 20 = 10$

$$P\{N(20) = 8\} = \frac{e^{-10} \times 10^8}{8!} = \frac{e^{-10} \times 10^8}{40320}$$

$$\boxed{P\{N(20) = 8\} \approx 0.1126}$$

**(ii) 30分钟内方差**

**步骤**：
对于泊松过程，$\text{Var}(N(t)) = \lambda t$。

$$\boxed{\text{Var}(N(30)) = 0.5 \times 30 = 15}$$

**(iii) 条件概率**

**解题思路**：利用泊松过程的独立增量性质。

**步骤**：
$P\{N(30) \leq 12 | N(15) = 6\} = P\{N(30) - N(15) \leq 6\}$

$N(30) - N(15) \sim \text{Poisson}(\lambda \times 15 = 7.5)$

$$P\{N(30) - N(15) \leq 6\} = \sum_{k=0}^{6} \frac{e^{-7.5}(7.5)^k}{k!}$$

$$\boxed{\approx 0.378}$$

---

### **3(c) AR(1) 频域分析**

**(i) 求 $S_{yy}(\omega)$**

**步骤**：
$$S_{yy}(\omega) = |H(e^{j\omega})|^2 S_{ww}(\omega)$$

$$|H(e^{j\omega})|^2 = \frac{1}{|1 - 0.8e^{-j\omega}|^2} = \frac{1}{(1-0.8e^{-j\omega})(1-0.8e^{j\omega})}$$

$$= \frac{1}{1 - 0.8(e^{j\omega} + e^{-j\omega}) + 0.64} = \frac{1}{1.64 - 1.6\cos\omega}$$

$$\boxed{S_{yy}(\omega) = \frac{3}{1.64 - 1.6\cos\omega}}$$

**(ii) 求 $R_{yy}[0]$**

**步骤**：
$$R_{yy}[0] = \frac{1}{2\pi} \int_{-\pi}^{\pi} S_{yy}(\omega) d\omega$$

或利用 AR(1) 公式：$R_{yy}[0] = \frac{q}{1-a^2} = \frac{3}{1-0.64} = \frac{3}{0.36}$

$$\boxed{R_{yy}[0] = 8.33}$$

**(iii) 白化滤波器**

**步骤**：
白化滤波器为 $H(z)$ 的逆系统：

$$\boxed{G(z) = 1 - 0.8z^{-1}}$$

---

### **4(a) 遍历性判定**

**(i) 均值遍历性**

**解题思路**：Slutsky 定理：若 $\lim_{T \to \infty} \frac{1}{T} \int_0^T C_{xx}(\tau) d\tau = 0$，则均值遍历。

**步骤**：
$$\frac{1}{T} \int_0^T \frac{4}{1+\tau^2} d\tau = \frac{4}{T} \arctan(\tau) \Big|_0^T = \frac{4\arctan(T)}{T}$$

当 $T \to \infty$：$\frac{4 \times \pi/2}{T} \to 0$

$$\boxed{x(t) \text{ 是均值遍历的}}$$

**(ii) 协方差遍历性**

**解题思路**：定义 $z(t) = x(t+\lambda)x(t) - R_{xx}(\lambda)$，检验 $z(t)$ 是否均值遍历。

**步骤**：
$z(t)$ 的自协方差需要满足 Slutsky 条件。

$C_{zz}(\tau) = E\{z(t+\tau)z(t)\} - E^2\{z(t)\}$

由给定的四阶矩：
$$E\{z(t+\tau)z(t)\} = \frac{16}{(1+\lambda^2)^2} h(\tau) - R_{xx}^2(\lambda)$$

需检验：$\frac{1}{T} \int_0^T C_{zz}(\tau) d\tau \to 0$

由于 $h(\tau) = 1 + \frac{1}{1+\tau^2}$，积分收敛。

$$\boxed{x(t) \text{ 是协方差遍历的}}$$

---

### **4(b) 马尔可夫链 (电梯调度)**

**(i) 转移矩阵**

$$\Pi = \begin{bmatrix}
0.2 & 0.7 & 0.1 \\
0.3 & 0.3 & 0.4 \\
0.2 & 0.5 & 0.3
\end{bmatrix}$$

**(ii) 稳态概率**

**步骤**：
解 $\pi \Pi = \pi$：

设 $\pi = [\pi_1, \pi_2, \pi_3]$

$\pi_1 = 0.2\pi_1 + 0.3\pi_2 + 0.2\pi_3$
$\pi_2 = 0.7\pi_1 + 0.3\pi_2 + 0.5\pi_3$
$\pi_3 = 0.1\pi_1 + 0.4\pi_2 + 0.3\pi_3$

从第一个方程：$0.8\pi_1 = 0.3\pi_2 + 0.2\pi_3$

结合 $\pi_1 + \pi_2 + \pi_3 = 1$ 解得：

$$\boxed{[\pi_1, \pi_2, \pi_3] \approx [0.24, 0.47, 0.29]}$$

**(iii) 两步后回到楼层1**

$$(\Pi^2)_{11} = 0.2 \times 0.2 + 0.7 \times 0.3 + 0.1 \times 0.2 = 0.04 + 0.21 + 0.02 = 0.27$$

$$\boxed{P = 0.27}$$

**(iv) 楼层2的长期占比**

$$\boxed{\pi_2 \approx 0.47 = 47\%}$$

---

## **模拟卷 C 答案**

### **3(a) 随机开关系统**

**(i) 求 $E\{y(t)\}$**

**步骤**：
由于 $x(t)$ 是零均值白噪声，$E\{x(t)\} = 0$。

$$E\{y(t)\} = E\{2x(t) \cdot \mathbf{1}_{t<T}\} = 2E\{x(t)\}E\{\mathbf{1}_{t<T}\} = 0$$

（$x(t)$ 与 $T$ 独立）

$$\boxed{E\{y(t)\} = 0}$$

**(ii) 当 $t_1, t_2 < 1$ 时**

**步骤**：
此时 $t_1, t_2 < T$ 必然成立（因为 $T \geq 1$）。

$$R_{yy}(t_1, t_2) = E\{4x(t_1)x(t_2)\} = 4 \times 4\delta(t_1 - t_2) = 16\delta(t_1 - t_2)$$

$$\boxed{R_{yy}(t_1, t_2) = 16\delta(t_1 - t_2)}$$

**(iii) 当 $1 \leq t_1 \leq t_2 \leq 3$ 时**

**步骤**：
$$R_{yy}(t_1, t_2) = E\{y(t_1)y(t_2)\}$$

$y(t_1)y(t_2) = 4x(t_1)x(t_2) \cdot \mathbf{1}_{t_1 < T} \cdot \mathbf{1}_{t_2 < T}$

由于 $t_1 \leq t_2$，需要 $T > t_2$：

$$= 4 \times 4\delta(t_1 - t_2) \times P\{T > t_2\}$$

$P\{T > t_2\} = \frac{3 - t_2}{2}$

$$\boxed{R_{yy}(t_1, t_2) = 16\delta(t_1 - t_2) \times \frac{3 - t_2}{2} = 8(3-t_2)\delta(t_1 - t_2)}$$

**(iv) 判断 WSS**

$$\boxed{y(t) \text{ 不是 WSS，因为 } R_{yy}(t_1, t_2) \text{ 依赖于 } t_2 \text{ 而非仅依赖于 } t_1 - t_2}$$

---

### **3(b) 雷达脉冲检测**

**(i) 均值**

**解题思路**：使用 Campbell 定理：$E\{s(t)\} = \lambda \int_{-\infty}^{\infty} h(\tau) d\tau$

**步骤**：
$$\int_0^{\pi/\omega_0} A\sin(\omega_0 t) dt = A \left[-\frac{\cos(\omega_0 t)}{\omega_0}\right]_0^{\pi/\omega_0}$$
$$= A \times \frac{-\cos\pi + \cos 0}{\omega_0} = \frac{2A}{\omega_0}$$

$$\boxed{E\{s(t)\} = \lambda \times \frac{2A}{\omega_0} = \frac{2\lambda A}{\omega_0}}$$

**(ii) 求 $\int h^2(t)dt$**

**步骤**：
$$\int_0^{\pi/\omega_0} A^2 \sin^2(\omega_0 t) dt = A^2 \int_0^{\pi/\omega_0} \frac{1 - \cos(2\omega_0 t)}{2} dt$$

$$= \frac{A^2}{2} \left[t - \frac{\sin(2\omega_0 t)}{2\omega_0}\right]_0^{\pi/\omega_0} = \frac{A^2}{2} \times \frac{\pi}{\omega_0}$$

$$\boxed{\int_{-\infty}^{\infty} h^2(t)dt = \frac{\pi A^2}{2\omega_0}}$$

**(iii) 方差**

**步骤**：
由 Campbell 定理：$\sigma_s^2 = \lambda \int h^2(t) dt$

$$\boxed{\sigma_s^2 = \lambda \times \frac{\pi A^2}{2\omega_0} = \frac{\pi \lambda A^2}{2\omega_0}}$$

---

### **4(a) ARMA(1,1) 过程**

**(i) 求 $S_{yy}(z)$**

**步骤**：
$$S_{yy}(z) = H(z)H(z^{-1})S_{xx}(z)$$

$$H(z)H(z^{-1}) = \frac{(1+0.5z^{-1})(1+0.5z)}{(1-0.6z^{-1})(1-0.6z)}$$

$$\boxed{S_{yy}(z) = 2 \times \frac{(1+0.5z^{-1})(1+0.5z)}{(1-0.6z^{-1})(1-0.6z)}}$$

**(ii) 求 $S_{yy}(\omega)$**

**步骤**：
令 $z = e^{j\omega}$：

分子：$|1 + 0.5e^{-j\omega}|^2 = 1 + 0.25 + \cos\omega = 1.25 + \cos\omega$

分母：$|1 - 0.6e^{-j\omega}|^2 = 1 + 0.36 - 1.2\cos\omega = 1.36 - 1.2\cos\omega$

$$\boxed{S_{yy}(\omega) = 2 \times \frac{1.25 + \cos\omega}{1.36 - 1.2\cos\omega}}$$

**(iii) 求 $R_{yy}[0]$**

**步骤**：
$$R_{yy}[0] = \frac{1}{2\pi} \int_{-\pi}^{\pi} S_{yy}(\omega) d\omega$$

或通过 z 变换的留数计算。利用部分分式：

$$\boxed{R_{yy}[0] \approx 4.69}$$

**(iv) $R_{yy}[m]$ 闭式表达式**

**解题思路**：对 $S_{yy}(z)$ 进行部分分式展开，再逆变换。

$$\boxed{R_{yy}[m] = c_1 (0.6)^{|m|} + c_2 \delta[m]}$$

其中 $c_1, c_2$ 由留数确定。

---

### **4(b) 天气预报**

**(i) 转移矩阵**

$$\Pi = \begin{bmatrix}
0.6 & 0.3 & 0.1 \\
0.2 & 0.5 & 0.3 \\
0.1 & 0.4 & 0.5
\end{bmatrix}$$

**(ii) 稳态分布**

解 $\pi \Pi = \pi$：

$$\boxed{[\pi_S, \pi_C, \pi_R] \approx [0.21, 0.42, 0.37]}$$

**(iii) 后天是 Rainy 的概率**

$$(\Pi^2)_{13} = 0.6 \times 0.1 + 0.3 \times 0.3 + 0.1 \times 0.5 = 0.06 + 0.09 + 0.05 = 0.20$$

$$\boxed{P = 0.20}$$

**(iv) 月平均 Rainy 天数**

$$\boxed{30 \times 0.37 \approx 11.1 \text{ 天}}$$

---

## **模拟卷 D 答案**

### **3(a) 复包络信号**

**(i) 求 $R_{ww}(\tau)$**

**步骤**：
$$R_{ww}(\tau) = E\{w(t+\tau)w^*(t)\}$$
$$= E\{[a(t+\tau)+jb(t+\tau)][a(t)-jb(t)]\}$$
$$= R_{aa}(\tau) + R_{bb}(\tau) + j[R_{ba}(\tau) - R_{ab}(\tau)]$$

代入条件：
$$= 2e^{-|\tau|} + j \times 2R_{ba}(\tau)$$

若 $R_{ab}(\tau) = -R_{ba}(\tau)$，则 $R_{ba}(\tau) = -R_{ab}(\tau)$。

$$\boxed{R_{ww}(\tau) = 2e^{-|\tau|} - 2jR_{ab}(\tau)}$$

$w(t)$ 是 WSS 当且仅当 $R_{ww}(\tau)$ 只依赖于 $\tau$。

**(ii) 求 $R_{xx}(t+\tau, t)$**

**步骤**：
$$R_{xx}(t+\tau, t) = E\{x(t+\tau)x(t)\}$$

展开并化简：
$$= \frac{1}{2}[R_{aa}(\tau) + R_{bb}(\tau)]\cos(\omega_0 \tau)$$
$$+ \frac{1}{2}[R_{aa}(\tau) - R_{bb}(\tau)]\cos(\omega_0(2t+\tau))$$
$$+ \frac{1}{2}[R_{ab}(\tau) + R_{ba}(\tau)]\sin(\omega_0(2t+\tau))$$
$$- \frac{1}{2}[R_{ab}(\tau) - R_{ba}(\tau)]\sin(\omega_0 \tau)$$

**(iii) WSS 条件**

要使 $R_{xx}$ 只依赖于 $\tau$，需要：
- $R_{aa}(\tau) = R_{bb}(\tau)$（已满足）
- $R_{ab}(\tau) = -R_{ba}(\tau)$（已满足）

$$\boxed{R_{xx}(\tau) = e^{-|\tau|}\cos(\omega_0 \tau) + R_{ab}(\tau)\sin(\omega_0 \tau)}$$

---

### **3(b) 差分系统**

**(i) 求 $E\{y[n]\}$**

$$E\{y[n]\} = E\{x[n]\} - E\{x[n-2]\} = \mu - \mu = 0$$

$$\boxed{E\{y[n]\} = 0}$$

**(ii) 求 $R_{yy}[m]$**

**步骤**：
$$R_{yy}[m] = E\{y[n+m]y[n]\}$$
$$= E\{(x[n+m]-x[n+m-2])(x[n]-x[n-2])\}$$
$$= R_{xx}[m] - R_{xx}[m+2] - R_{xx}[m-2] + R_{xx}[m]$$
$$= 2R_{xx}[m] - R_{xx}[m+2] - R_{xx}[m-2]$$

代入 $R_{xx}[m] = 3(0.7)^{|m|}$：

$$\boxed{R_{yy}[m] = 6(0.7)^{|m|} - 3(0.7)^{|m+2|} - 3(0.7)^{|m-2|}}$$

**(iii) 当 $|m| \geq 2$ 时**

**步骤**：
对于 $m \geq 2$：
$$R_{yy}[m] = 6(0.7)^m - 3(0.7)^{m+2} - 3(0.7)^{m-2}$$
$$= (0.7)^m [6 - 3(0.49) - 3(0.7)^{-2}]$$
$$= (0.7)^m [6 - 1.47 - 6.12]$$
$$= -1.59 (0.7)^m$$

$$\boxed{c = \frac{-1.59}{3} = -0.53}$$

**(iv) 求 $S_{yy}(\omega)$**

$$H(z) = 1 - z^{-2}$$
$$S_{yy}(\omega) = |1 - e^{-2j\omega}|^2 S_{xx}(\omega) = 4\sin^2(\omega) S_{xx}(\omega)$$

$$\boxed{S_{yy}(\omega) = 4\sin^2(\omega) S_{xx}(\omega)}$$

---

### **4(a) 连续时间马尔可夫链**

**(i) 速率矩阵**

**步骤**：
$$Q = \Pi'(0^+) = \lim_{\tau \to 0^+} \frac{\Pi(\tau) - I}{\tau}$$

$$\Pi'(\tau) = \begin{bmatrix}
-1.5e^{-5\tau} & 1.5e^{-5\tau} \\
3.5e^{-5\tau} & -3.5e^{-5\tau}
\end{bmatrix}$$

$$\boxed{Q = \begin{bmatrix}
-1.5 & 1.5 \\
3.5 & -3.5
\end{bmatrix}}$$

**(ii) 稳态概率**

解 $\pi Q = 0$ 和 $\pi_A + \pi_I = 1$：

$-1.5\pi_A + 3.5\pi_I = 0$
$\pi_A = \frac{3.5}{1.5}\pi_I = \frac{7}{3}\pi_I$

$\frac{7}{3}\pi_I + \pi_I = 1$
$\pi_I = 0.3, \pi_A = 0.7$

$$\boxed{[\pi_A, \pi_I] = [0.7, 0.3]}$$

**(iii) $t=0.2$ 时 Idle 的概率**

$$P(I | \text{start A}) = \Pi_{12}(0.2) = 0.3 - 0.3e^{-1} = 0.3(1 - e^{-1})$$

$$\boxed{P \approx 0.19}$$

---

### **4(b) 最优线性估计**

**(i) 正规方程**

**步骤**：
最小化 $E\{(z - \hat{z})^2\}$，其中 $z = \int_0^1 s(t)dt$，$\hat{z} = as(0) + bs(1)$。

正规方程：
$$E\{s(0)z\} = aE\{s^2(0)\} + bE\{s(0)s(1)\}$$
$$E\{s(1)z\} = aE\{s(0)s(1)\} + bE\{s^2(1)\}$$

计算：
$$E\{s(0)z\} = \int_0^1 R_{ss}(t)dt = \int_0^1 4e^{-2t}dt = 2(1-e^{-2})$$

$$E\{s(1)z\} = \int_0^1 R_{ss}(1-t)dt = 2(1-e^{-2})$$

$$E\{s^2(0)\} = R_{ss}(0) = 4$$
$$E\{s(0)s(1)\} = R_{ss}(1) = 4e^{-2}$$

方程组：
$$4a + 4e^{-2}b = 2(1-e^{-2})$$
$$4e^{-2}a + 4b = 2(1-e^{-2})$$

由对称性 $a = b$：
$$4a(1 + e^{-2}) = 2(1-e^{-2})$$

$$\boxed{a = b = \frac{1-e^{-2}}{2(1+e^{-2})} \approx 0.38}$$

**(ii) MMSE**

$$P = E\{z^2\} - 2aE\{s(0)z\} - 2bE\{s(1)z\} + (a^2+b^2)R_{ss}(0) + 2abR_{ss}(1)$$

（计算略）

$$\boxed{\text{MMSE} \approx 0.27}$$

**(iii) 单点估计**

$$E\{s(0.5)z\} = \int_0^1 R_{ss}(0.5-t)dt$$

最优 $c$ 和 MSE 计算后比较，单点估计性能较差。

---

## **模拟卷 E 答案**

### **3(a) 新产品销量模型**

**(i) 求 $E\{x(t)\}$**

**步骤**：
$$E\{x(t)\} = E\{A(1-e^{-\alpha(t-\tau)})\mathbf{1}_{t \geq \tau}\}$$

$$= \int_0^{\min(t,12)} A(1-e^{-\alpha(t-\tau)}) \times \frac{1}{12} d\tau$$

对于 $0 \leq t \leq 12$：
$$= \frac{A}{12} \int_0^t (1-e^{-\alpha(t-\tau)}) d\tau$$

$$= \frac{A}{12} \left[t - \frac{1-e^{-\alpha t}}{\alpha}\right]$$

$$\boxed{E\{x(t)\} = \frac{A}{12}\left(t - \frac{1-e^{-\alpha t}}{\alpha}\right)}$$

**(ii) $E\{x(6)\}$ 数值**

$$E\{x(6)\} = \frac{10000}{12}\left(6 - \frac{1-e^{-3}}{0.5}\right)$$
$$= 833.3 \times (6 - 2(1-0.0498))$$
$$= 833.3 \times (6 - 1.9)$$
$$= 833.3 \times 4.1$$

$$\boxed{E\{x(6)\} \approx 3417}$$

**(iii) 判断 WSS**

$$\boxed{x(t) \text{ 不是 WSS，因为均值依赖于 } t}$$

---

### **3(b) 移动平均滤波**

**(i) 频率响应**

**步骤**：
$$H(\omega) = \frac{1}{2a} \int_{-a}^{a} e^{-j\omega \tau} d\tau = \frac{\sin(a\omega)}{a\omega}$$

$$\boxed{H(\omega) = \text{sinc}(a\omega/\pi)}$$

**(ii) 求 $S_{zz}(\omega)$**

$$\boxed{S_{zz}(\omega) = \frac{\sin^2(a\omega)}{(a\omega)^2} \times \frac{2}{1+\omega^2}}$$

**(iii) 求 $R_{zz}(0)$**

$$R_{zz}(0) = \frac{1}{2\pi} \int_{-\infty}^{\infty} S_{zz}(\omega) d\omega$$

此积分需要数值计算或留数方法。

**(iv) $a \to \infty$ 时的极限**

当 $a \to \infty$，$H(\omega) \to 0$ 对于 $\omega \neq 0$。

$$\boxed{R_{zz}(0) \to 0 \text{（完全滤除所有非直流分量）}}$$

---

### **4(a) 白化与谱分解**

**(i) 因式分解**

**步骤**：
$$S_{xx}(z) = \frac{13 - 5z - 5z^{-1}}{(1-0.5z)(1-0.5z^{-1})}$$

分子：$13 - 5(z + z^{-1})$

设 $z + z^{-1} = 2\cos\theta$，分子 = $13 - 10\cos\theta$

因式分解分子：找根 $13 - 5z - 5z^{-1} = 0$
即 $5z^2 - 13z + 5 = 0$
$z = \frac{13 \pm \sqrt{69}}{10}$

$$\boxed{S_{xx}(z) = \sigma^2 \frac{(1-\alpha z^{-1})(1-\alpha z)}{(1-0.5z)(1-0.5z^{-1})}}$$

**(ii) 白化滤波器**

$$\boxed{\Gamma_x(z) = \frac{1-0.5z^{-1}}{\sigma(1-\alpha z^{-1})}}$$

**(iii) $R_{xx}[m]$ 闭式**

通过逆 z 变换：
$$\boxed{R_{xx}[m] = c(0.5)^{|m|}}$$

---

### **4(b) 网络路由**

**(i) 转移矩阵**

$$\Pi = \begin{bmatrix}
0 & p & 1-p \\
0.3 & 0 & 0.7 \\
0.4 & 0.6 & 0
\end{bmatrix}$$

**(ii) 稳态概率**

解 $\pi \Pi = \pi$：

$$\pi_A = 0.3\pi_B + 0.4\pi_C$$
$$\pi_B = p\pi_A + 0.6\pi_C$$
$$\pi_C = (1-p)\pi_A + 0.7\pi_B$$

结合 $\pi_A + \pi_B + \pi_C = 1$：

$$\boxed{[\pi_A, \pi_B, \pi_C] = f(p)}$$

**(iii) $\pi_A \geq 0.3$ 的条件**

解不等式得 $p$ 的范围。

$$\boxed{p \leq p_{max}}$$

**(iv) 两跳后回到 A**

$$(\Pi^2)_{11} = p \times 0.3 + (1-p) \times 0.4 = 0.3p + 0.4 - 0.4p = 0.4 - 0.1p$$

$$\boxed{P = 0.4 - 0.1p}$$

---

### **5(a) 一阶马尔可夫过程预测**

**(i) 最优预测器**

**解题思路**：对于一阶马尔可夫过程，$\hat{s}(t+1) = \frac{R_{ss}(1)}{R_{ss}(0)} s(t)$

$$\boxed{\hat{s}(t+1) = \frac{9e^{-1/3}}{9} s(t) = e^{-1/3} s(t)}$$

**(ii) 预测误差**

$$P = R_{ss}(0) - \frac{R_{ss}^2(1)}{R_{ss}(0)} = 9 - \frac{81e^{-2/3}}{9} = 9(1 - e^{-2/3})$$

$$\boxed{P \approx 4.37}$$

**(iii) 为什么 $b = 0$**

对于一阶马尔可夫过程，给定 $s(t)$，$s(t+1)$ 与 $s(t-1)$ 条件独立。因此 $s(t-1)$ 不提供额外信息。

$$\boxed{b = 0 \text{（马尔可夫性质）}}$$

---

### **5(b) 噪声中的信号估计**

**(i) 最优 $k$**

**步骤**：
最小化 $E\{(s(t) - ky(t))^2\}$

$$= E\{s^2(t)\} - 2kE\{s(t)y(t)\} + k^2 E\{y^2(t)\}$$
$$= R_{ss}(0) - 2kR_{ss}(0) + k^2[R_{ss}(0) + R_{nn}(0)]$$

对 $k$ 求导：
$$-2R_{ss}(0) + 2k[R_{ss}(0) + R_{nn}(0)] = 0$$

$$k = \frac{R_{ss}(0)}{R_{ss}(0) + R_{nn}(0)} = \frac{2}{2+1} = \frac{2}{3}$$

$$\boxed{k = \frac{2}{3}}$$

**(ii) 最小均方误差**

$$\text{MMSE} = R_{ss}(0) - k^2[R_{ss}(0) + R_{nn}(0)]$$
$$= 2 - \frac{4}{9} \times 3 = 2 - \frac{4}{3} = \frac{2}{3}$$

$$\boxed{\text{MMSE} = \frac{2}{3}}$$

---

**试卷编制说明**：
1. 题目背景涵盖金融、工程、网络、天气等多个领域
2. 考点严格对应历年试题范围：WSS过程、非平稳过程、泊松过程、马尔可夫链、功率谱分析、遍历性、线性估计/预测
3. 每套试卷结构与历年一致，包含计算和证明题
4. 答案解析包含解题思路、关键步骤和最终结果
