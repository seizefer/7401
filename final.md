### 

**2025A**

**1. (a)**  
Consider a 6-sided die with faces numbered 1 to 6. It is tossed twice independently and for each toss the number on the top face is recorded. Define the following events:  

- \( A \): the number on the first toss is even.  
- \( B \): the number on the second toss is even.  
- \( C \): the product of the numbers from both tosses is even.  
- \( D \): the numbers from both tosses are even.  

Is it true that \(\mathbb{P}(D \mid A) \geq \mathbb{P}(D \mid C)\)? Justify your answer. Note that it is not assumed that the die is fair.  
*(10 Marks)*

**(b)**  
A coin with probability \( p \) of heads is tossed until the first tail appears. If the number of tosses in this procedure is \( n \), you receive \( 2^n \) dollars. What is the expected amount of money (as a function of \( p \)) you will receive?  
*(10 Marks)*

**(c)**  
The number of cats within any distance \( r \) from Canteen B is modeled as a random variable \( N \) with probability mass function (pmf)  
\[
\mathbb{P}(N = n \mid r) = \frac{1}{n!} e^{-\lambda \pi r^2} (\lambda \pi r^2)^n, \quad n = 0, 1, \ldots
\]  
Here, \( \lambda \) is a positive constant. Let \( X \) be the distance from Canteen B to the nearest cat. Find the probability density function (pdf) of \( X \).  
*Hint: find the cumulative distribution function (cdf) first.*  
*(10 Marks)*

**2.**  
The random variables \( X \), \( H \), and \( Z \) in Figure 1 are independent. Suppose that \( X \) and \( Z \) are zero-mean random variables with variances \( P \) and \( N \), respectively. The multiplicative noise \( H \) has mean \( m \) and variance \( \sigma^2 \).  

**Figure 1**  
\( X \rightarrow H \rightarrow Z \)  
\( X \rightarrow X \rightarrow Y = HX + Z \)  

**(a)** Find the mean and variance of \( Y \).  
**(b)** Find the covariance between \( X \) and \( Y \).  
**(c)** Find the minimum mean-square error (MMSE) linear estimate of \( X \) given \( Y \) and the mean-square error (MSE).  
**(d)** Suppose that \( m = 1 \). Is the MSE you obtained in part (c) smaller than the MMSE of the case where there is no multiplicative noise, i.e., \( H \equiv 1 \)? Justify your answer.  
*(5 Marks)*

---

### 关键条件复述（中文）

**1(a)**  
- 一个6面骰子（点数1–6），独立投掷两次。  
- 事件定义：  
  - \( A \)：第一次投掷点数为偶数  
  - \( B \)：第二次投掷点数为偶数  
  - \( C \)：两次投掷点数的乘积为偶数  
  - \( D \)：两次投掷点数均为偶数  
- 问题：判断是否 \( \mathbb{P}(D \mid A) \geq \mathbb{P}(D \mid C) \)，骰子不一定均匀。

**1(b)**  
- 一枚硬币，正面概率 \( p \)，反复投掷直到第一次出现反面，设投掷次数为 \( n \)。  
- 获得奖金 \( 2^n \) 美元。  
- 求期望奖金（关于 \( p \) 的函数）。

**1(c)**  
- 在距离Canteen B为 \( r \) 的范围内，猫的数量 \( N \) 服从泊松分布：  
  \[
  \mathbb{P}(N = n \mid r) = \frac{1}{n!} e^{-\lambda \pi r^2} (\lambda \pi r^2)^n
  \]  
- \( X \) 表示到最近一只猫的距离。  
- 求 \( X \) 的概率密度函数（提示：先求累积分布函数）。

**2**  
- 独立随机变量：\( X, H, Z \)。  
- \( X, Z \) 均值为0，方差分别为 \( P, N \)。  
- \( H \) 均值为 \( m \)，方差为 \( \sigma^2 \)。  
- 系统模型：\( Y = HX + Z \)。  
- 要求：  
  - (a) \( Y \) 的均值和方差  
  - (b) \( X \) 与 \( Y \) 的协方差  
  - (c) 给定 \( Y \) 时 \( X \) 的MMSE线性估计及其MSE  
  - (d) 若 \( m = 1 \)，比较有乘性噪声 \( H \) 与无乘性噪声（\( H \equiv 1 \)）时的MSE大小。



### （续）

**3. (a)**  
*Warning:* Since Sands and Resorts World opened their doors, Mr. Won Ah Lot has won a lot of money. His total winning at time \(t\) may be modelled as a real non-stationary process \(x(t)\). \(x(t)\) is defined only for \(t\geq 0\). Mr. Won starts with no winning, or \(x(0)=0\). \(x(t)\) has two properties.  
(1) Mr. Won's luck during one interval is independent of another interval, or the change of his total winning in two non-overlapping intervals are uncorrelated, i.e.,  
\[
E\left([x(t_{4})-x(t_{3})][x(t_{2})-x(t_{1})]\right)=0 \quad \text{for any } 0\leq t_{1}\leq t_{2}\leq t_{3}\leq t_{4}.
\]  
(2) On an average, the square of the change of Mr. Won's total winning in one interval is proportional to the length of the time interval, i.e.,  
\[
E\left([x(t_{2})-x(t_{1})]^{2}\right)=10(t_{2}-t_{1}) \quad \text{for any } 0\leq t_{1}\leq t_{2}.
\]  
In the following, help Mr. Won find \(R_{xx}(t_{1},t_{2})\), the autocorrelation of \(x(t)\).  

(i) Using \(x(0)=0\) on property (1), show that \(R_{xx}(t_{2},t_{3})-R_{xx}(t_{2},t_{1})=0\) for any \(0\leq t_{1}\leq t_{2}\leq t_{3}\).  

(ii) Using the result of part 3(a)(i) on property (2), find \(R_{xx}(t_{2},t_{3})\) for any \(0\leq t_{2}\leq t_{3}\).  

(iii) Combining the results of parts 3(a)(i) and 3(a)(ii), find \(R_{xx}(t_{1},t_{2})\) for any \(t_{1},t_{2}\).  
*(12 Marks)*

**(b)**  
*Alternate measure:* \(y(t)\) is a real WSS (wide sense stationary) process with an unknown power spectrum \(S_{yy}(\omega)\). Since \(y(t)\) cannot be measured directly, NTU researcher Li Mei Si measures \(s(t)=y(t+a)+y(t-a)\), or the sum of two values of \(y(t)\) that are \(2a\) apart. Her co-researcher Macy Lee prefers to measure \(d(t)=y(t+a)-y(t-a)\), or the difference of the same two values of \(y(t)\).  

(i) How correlated are Mei Si's and Macy's measured processes at the same time? Find \(R_{sd}(t,t)\), the cross-correlation between \(s(t)\) and \(d(t)\) at the same time \(t\).  

(ii) Show that the power spectrum of Mei Si's measured process \(s(t)\) is given by \(S_{ss}(\omega)=4\cos^{2}(a\omega)S_{yy}(\omega)\).  

(iii) Find \(S_{dd}(\omega)\), the power spectrum of Macy's measured process \(d(t)\).  

(iv) If it is known that the noise \(y(t)\) has frequencies at or near \(\omega=10\) radians, and the value of \(a\) used by both Mei Si and Macy is \(0.3\), then which among \(s(t)\) and \(d(t)\) will be a better measurement? *Hint: Compare the power spectrums obtained in parts 3(b)(ii) and 3(b)(iii) at or near \(\omega=10\) radians.*  

[You may find some of the following results useful. Recall that if a linear system has input \(y(t)\) and output \(y(t+a)\), then the frequency response of the linear system is \(e^{j\omega a}\). The time shift property states that if the Fourier transform of \(R(\tau)\) is \(S(\omega)\), then the Fourier transform of \(R(\tau-a)\) is \(e^{-j\omega a}S(\omega)\). Euler's formula is \(e^{j\theta}+e^{-j\theta}=2\cos(\theta)\) and \(e^{j\theta}-e^{-j\theta}=2j\sin(\theta)\). A trigonometric identity is \(\cos(2\theta)=1-2\sin^{2}(\theta)=2\cos^{2}(\theta)-1.]  
*(13 Marks)*

**4. (a)**  
*AR(1) process revisited:* In the lectures, we derived the autocorrelation of the AR(1) process using the \(z\)-transform. Here, we will derive the same result using the time-domain approach. Let \(x[n]\) be a real discrete-time WSS white noise process with autocorrelation  
\[
R_{xx}[n_{1},n_{2}]=q\delta[n_{1}-n_{2}]=\left\{\begin{array}{ll}q & n_{1}= n_{2},\\ 0 & n_{1}\neq n_{2},\end{array}\right.
\]  
where \(q\) is a positive constant, and \(\delta[\cdot]\) denotes discrete-time impulse. \(x[n]\) is passed through a linear system to obtain the output process \(y[n]\), also known as the AR(1) process. The linear system is characterized by the input-output relation \(y[n]=x[n]+ay[n-1]\) for all \(n\), where \(a\) is a real constant with \(|a|<1\).  

(i) Starting from the input-output relation \(y[n]=x[n]+ay[n-1]\), show that \(y[n]=\sum_{k=0}^{\infty}a^{k}x[n-k]\).  

(ii) In the following steps, we find the autocorrelation of the AR(1) process \(y[n]\), \(R_{yy}[n_{1},n_{2}]=E\{y[n_{1}]y[n_{2}]\}\). For the case \(n_{1}\leq n_{2}\), replace \(y[n_{1}]\) and \(y[n_{2}]\) in \(E\{y[n_{1}]y[n_{2}]\}\) by the summation result proved in part 4(a)(i). Evaluate and simplify the expectation into a closed form (i.e., no summation).  

(iii) Now for the case \(n_{1}>n_{2}\), again replace \(y[n_{1}]\) and \(y[n_{2}]\) in \(E\{y[n_{1}]y[n_{2}]\}\) by the summation result proved in part 4(a)(i). Evaluate and simplify the expectation into a closed form (i.e., no summation).  
*(12 Marks)*

**(b)**  
*Dementia:* Prof. Dame N. Seah is suffering from dementia. She usually keeps her glasses in her handbag, but she often forgets and keeps the glasses in her pocket. When Prof. Seah takes the glasses from the handbag and uses the glasses, she puts the glasses back into the handbag with probability 0.2. However, when Prof. Seah takes the glasses from her pocket, she puts the glasses back to the handbag with probability 0.4.  

(i) Formulate the above problem as a discrete-time finite state Markov chain, where the states represent whether the glasses are kept in the handbag or in the pocket. Draw the Markov chain diagram. Find the transition matrix for one state transition.  

(ii) When Prof. Seah needs her glasses, she always searches the handbag first. Only when she does not find the glasses in the handbag, she remembers to search her pocket. Find \(p_{pocket}\), the probability that on average she will find the glasses in the pocket when she need the glasses. (\(p_{pocket}\) is the steady state probability that the glasses are kept in the pocket.)  

(iii) If the probability she takes the glasses from the pocket and puts the glasses back to the handbag is increased from 0.4, explain if \(p_{pocket}\) will also increase or not.  
*(13 Marks)*

---

### 关键条件复述（中文）

**3(a)**  
- 过程 \(x(t)\) 表示 Mr. Won 在时间 \(t\) 的累计赢钱额，\(x(0)=0\)。  
- 性质 (1)：非重叠区间的增量不相关  
  \[
  E\left([x(t_{4})-x(t_{3})][x(t_{2})-x(t_{1})]\right)=0, \quad 0\leq t_{1}\leq t_{2}\leq t_{3}\leq t_{4}
  \]  
- 性质 (2)：增量平方的期望与时间长度成正比  
  \[
  E\left([x(t_{2})-x(t_{1})]^{2}\right)=10(t_{2}-t_{1}), \quad 0\leq t_{1}\leq t_{2}
  \]  
- 要求求自相关函数 \(R_{xx}(t_{1},t_{2})=E[x(t_{1})x(t_{2})]\)。

**3(b)**  
- \(y(t)\) 是实 WSS 过程，功率谱未知。  
- 测量信号：  
  \[
  s(t)=y(t+a)+y(t-a), \quad d(t)=y(t+a)-y(t-a)
  \]  
- 要求：  
  - (i) 求 \(R_{sd}(t,t)\)（同一时刻的互相关）  
  - (ii) 证明 \(S_{ss}(\omega)=4\cos^{2}(a\omega)S_{yy}(\omega)\)  
  - (iii) 求 \(S_{dd}(\omega)\)  
  - (iv) 已知 \(y(t)\) 的频率在 \(\omega\approx 10\) rad/s，\(a=0.3\)，比较 \(s(t)\) 与 \(d(t)\) 哪个更好。

**4(a)**  
- \(x[n]\) 是实离散时间白噪声，自相关为 \(R_{xx}[n_1,n_2]=q\delta[n_1-n_2]\)。  
- 系统：\(y[n]=x[n]+a y[n-1]\)，\(|a|<1\)。  
- 要求：  
  - (i) 证明 \(y[n]=\sum_{k=0}^{\infty}a^{k}x[n-k]\)  
  - (ii) 当 \(n_1\leq n_2\)，求 \(R_{yy}[n_1,n_2]\) 的闭式  
  - (iii) 当 \(n_1>n_2\)，求 \(R_{yy}[n_1,n_2]\) 的闭式

**4(b)**  
- Prof. Seah 放眼镜的位置：手提包（handbag）或口袋（pocket）。  
- 从手提包取出使用后，放回手提包的概率 = 0.2。  
- 从口袋取出使用后，放回手提包的概率 = 0.4。  
- 要求：  
  - (i) 建立两状态马尔可夫链，画图，求转移矩阵  
  - (ii) 求稳态概率 \(p_{pocket}\)（平均在口袋中找到眼镜的概率）  
  - (iii) 若从口袋放回手提包的概率从 0.4 增加，解释 \(p_{pocket}\) 是否增加。





**2024**



### 

**1. (a)**  
Adrian uses a ride hailing app to book a ride. With probability \( 1/4 \), a driver is assigned immediately by the app. Otherwise, he waits for a driver to be found in a time that is uniformly distributed between 1 and 3 minutes. Let \( X \) be Adrian’s waiting time. Find the cumulative distribution function (cdf) and the expected value of \( X \).  
*(6 Marks)*

**(b)**  
It is known that a newly discovered drug has a probability \( P \) of treating COVID-19. The value of \( P \) is unknown but assumed to be uniformly distributed in \([0, 1]\). A clinical trial is conducted in which it is observed that the drug is effective in \( X = 14 \) out of 15 patients. Assuming that the drug acts independently on each patient, find the posterior probability \( f_{P|X}(p | 14) \).  
*(6 Marks)*

**(c)**  
Suppose that \( X \sim \mathcal{N}(0, 1) \) is a standard normal random variable.  

(i) Using integration by parts, show that for each integer \( n \geq 2 \), we have  
\[
\mathbb{E}[X^n] = (n - 1)\mathbb{E}[X^{n-2}].
\]  

(ii) Show that if \( n \) is odd, \( \mathbb{E}[X^n] = 0 \).  

(iii) Show that if \( n \) is even, \( \mathbb{E}[X^n] = (n - 1)(n - 3) \cdots 1 \).  

(Hint: For parts (ii) and (iii), use mathematical induction.)  
*(13 Marks)*

**2. (a)**  
Let \( \mathbf{X} = \begin{bmatrix} X_1 \\ X_2 \\ X_3 \end{bmatrix} \) be a zero-mean Gaussian random vector with distribution \( \mathcal{N}(0, \Sigma) \), where  
\[
\Sigma = \begin{bmatrix} 2 & 1 & 1 \\ 1 & 4 & 1 \\ 1 & 1 & 2 \end{bmatrix}.
\]  
Express your answers to the following questions in the format \( \mathcal{N}(\mu', \Sigma') \) by writing down explicitly the values of \( \mu' \) and \( \Sigma' \).  

(i) What is the probability density function (pdf) of \( X_3 \) given \( (X_1, X_2) \)?  

(ii) What is the joint pdf of \( Y = AX \), where  
\[
A = \begin{bmatrix} 1 & 3 & -1 \\ 2 & 1 & -1 \end{bmatrix}?
\]  
*(10 Marks)*

**(b)**  
Consider the Gaussian random vector \( X \) in part (a). Find the minimum mean-square error (MMSE) estimate of \( Y = \mathbb{E}[X_3 | X_2] \) given \( X_1 \) and its MSE.  
*(5 Marks)*

**(c)**  
Suppose that \( U \) and \( V \) are jointly Gaussian and uncorrelated. Is it true that \( \mathbb{E}[U^3V^3] = \mathbb{E}[U^3]\mathbb{E}[V^3] \)? Justify your answer.  
*(5 Marks)*

---

### 关键条件复述（中文）

**1(a)**  
- Adrian 使用打车软件叫车。  
- 以概率 \(1/4\)，司机立即被分配（等待时间 = 0）。  
- 否则，等待时间服从 [1,3] 分钟上的均匀分布。  
- 设 \(X\) 为等待时间，求其累积分布函数（cdf）和期望值。

**1(b)**  
- 一种新药治疗 COVID-19 的有效概率为 \(P\)。  
- \(P\) 的先验分布为 \([0,1]\) 上的均匀分布。  
- 临床试验中 15 名患者有 14 名有效（\(X=14\)）。  
- 假设对每位患者作用独立，求后验概率密度函数 \(f_{P|X}(p | 14)\)。

**1(c)**  
- \(X \sim \mathcal{N}(0, 1)\) 是标准正态随机变量。  
- (i) 用分部积分证明：对所有整数 \(n \geq 2\)，有 \(\mathbb{E}[X^n] = (n - 1)\mathbb{E}[X^{n-2}]\)。  
- (ii) 证明若 \(n\) 为奇数，则 \(\mathbb{E}[X^n] = 0\)。  
- (iii) 证明若 \(n\) 为偶数，则 \(\mathbb{E}[X^n] = (n - 1)(n - 3) \cdots 1\)。  
- 提示：(ii)(iii) 用数学归纳法。

**2(a)**  
- 零均值高斯随机向量 \(\mathbf{X} = [X_1, X_2, X_3]^T \sim \mathcal{N}(0, \Sigma)\)，其中  
\[
\Sigma = \begin{bmatrix} 2 & 1 & 1 \\ 1 & 4 & 1 \\ 1 & 1 & 2 \end{bmatrix}.
\]  
- (i) 求给定 \((X_1, X_2)\) 时 \(X_3\) 的条件概率密度函数（pdf），答案写成 \(\mathcal{N}(\mu', \Sigma')\) 形式。  
- (ii) 求 \(Y = AX\) 的联合 pdf，其中  
\[
A = \begin{bmatrix} 1 & 3 & -1 \\ 2 & 1 & -1 \end{bmatrix}.
\]  
答案也写成 \(\mathcal{N}(\mu', \Sigma')\) 形式。

**2(b)**  
- 考虑 (a) 中的高斯随机向量 \(X\)。  
- 求给定 \(X_1\) 时，对 \(Y = \mathbb{E}[X_3 | X_2]\) 的最小均方误差（MMSE）估计，并求其均方误差（MSE）。

**2(c)**  
- 假设 \(U\) 和 \(V\) 是联合高斯且不相关的。  
- 问是否一定有 \(\mathbb{E}[U^3V^3] = \mathbb{E}[U^3]\mathbb{E}[V^3]\)？证明你的答案。







### 

**3. (a)**  
At the start, a sound system was not connected to any source. The input sound, therefore, was just system noise. Let this system noise be a real wide sense stationary (WSS) white noise process \(x(t)\). The autocorrelation of \(x(t)\) is \(R_{xx}(t_1,t_2)=5\delta(t_1-t_2)\), where \(\delta(t)\) denotes the continuous-time impulse function. Since the amplifier gain was 1, the output sound was inaudible. DJ Rong Song wanted to play a song, so he increased the amplifier gain to 100 at time \(t=0\). But he forgot to connect the source. To everyone’s surprise, loud noise came out of the sound system. Rong Song realized that he is playing the wrong song. At time \(t=2\), he decreased the amplifier gain to 1. Let the output sound be another process  
\[
y(t)=\begin{cases} 100x(t) & 0 \leq t \leq 2 \\ x(t) & \text{otherwise} \end{cases}.
\]  
Find \(R_{yy}(t_1,t_2)\), the autocorrelation of \(y(t)\), for the following 3 cases:  

(i) When both \(t_1\), \(t_2\) are inside the interval [0, 2].  
(ii) When one of \(t_1\), \(t_2\) is inside the interval [0, 2] but the other is outside.  
(iii) When both \(t_1\), \(t_2\) are outside the interval [0, 2].  

Using your result, determine if the output sound \(y(t)\) is WSS. (Hint: check if \(R_{yy}(t_1,t_2)\) depends only on \(t_1-t_2\).) Also determine if \(y(t)\) is white noise. (Hint: check if \(R_{yy}(t_1,t_2)\) is of the form \(q(t_1)\delta(t_1-t_2)\) for some \(q(t_1)\geq 0\).)  
*(10 Marks)*

**(b)**  
Waiting at the NTU bus stop, Goh Wen wonders when he will be able to go back. He knows that the number of arrivals from time 0 to \(t\) (measured in minutes), denoted by \(w(t)\), is a Poisson process with probability of \(k\) arrivals given by  
\[
P\{w(t)=k\} = \frac{e^{-\lambda t}(\lambda t)^k}{k!}.
\]  
Goh Wen also observed that there is 1 expected arrival in 5 minutes, or \(E\{w(5)\}=1\). However, most buses are so crowded that, Goh Wen figures, it would take him at least 2 arrivals before he has a chance to board the bus, and perhaps 4 arrivals to guarantee he will get in. He wants to go within 10 minutes. When will Goh Wen go? Let us do some calculations.  

(i) Find the numerical value of the probability that there are 2 to 4 arrivals within 10 minutes, or \(P\{2 \leq w(10) \leq 4\}\).  
(ii) To measure how uncertain the number of arrivals in 10 minutes is, find the numerical value of the variance of \(w(10)\).  
*(5 Marks)*

**(c)**  
A real stationary discrete-time white noise process \(x[n]\) has power spectrum \(S_{xx}(\omega)=2\). \(x[n]\) is passed through a linear system with transfer function  
\[
H(z) = \frac{1}{1 - 0.5z^{-1}}
\]  
to obtain an AR(1) process \(y[n]\). Find \(S_{yy}(\omega)\), the power spectrum of the AR(1) process \(y[n]\), and show that it is a real function.  
*(5 Marks)*

**4. (a)**  
_Car’s horse power:_ Since Singapore COE depends on the engine horse power, LTA officer Harsh Pawar calculates the horse power of a car from its acceleration under test conditions. \(x(t)\), a real stationary zero mean random process, denotes the acceleration over time. Mr. Pawar needs the mean and the covariance of \(x(t)\) for his calculation. He uses the time average of \(x(t)\) to estimate these. However, the process needs to be ergodic for Harsh Pawar to justify doing that.  

(i) Given that \(x(t)\)’s autocovariance is \(C_{xx}(\tau) = e^{-|\tau|}\), determine whether \(x(t)\) is mean-ergodic or not. (Hint: Use Slutsky’s theorem.)  

(ii) Further, Harsh Pawar knows that \(x(t)\)’s fourth order moment is  
\[
E\{x(t + \lambda + \tau)x(t + \tau)x(t + \lambda)x(t)\} = e^{-2|\lambda|}g(\tau),
\]  
where \(g(\tau)\) is given by:  
\[
g(\tau) = \begin{cases} 3 - |\tau| & |\tau| < 1, \\ \frac{|\tau|+1}{|\tau|} & 1 \leq |\tau|. \end{cases}
\]  
Find whether \(x(t)\) is covariance-ergodic or not. (Hint: Appropriately define another process \(z(t)\) such that \(x(t)\) is covariance-ergodic iff \(z(t)\) is mean-ergodic, and apply Slutsky’s theorem on \(z(t)\).)  
*(10 Marks)*

**(b)**  
_Dementia:_ Professor Dame N. Seah is suffering from dementia and keeps forgetting her umbrellas in the MRT. Professor Seah has 3 umbrellas in her home on Monday morning before she starts her MRT trip. Every morning it rains with a probability of 0.2. If it rains, and if Professor Seah still has any umbrella, she takes an umbrella to walk from her home to the MRT. She forgets the umbrella in the MRT. If it doesn’t rain, she doesn’t take any umbrella.  

(i) Formulate the above problem as a Markov chain, where the states represent the number of umbrellas Professor Dame N. Seah has at her home on any morning before she starts. (Hint: State 0 means no more umbrella to forget, so state 0 doesn’t have any transition to any other state.) Draw the discrete-time Markov chain. Label the transitions with the transition probabilities.  

(ii) Find the transition matrix \(\Pi[1]\) for this Markov chain.  

(iii) It is known that on Monday morning before her start, Professor Dame N. Seah has 3 umbrellas, or the Markov chain is initially in state 3. What is the probability that on Thursday morning before her start (that is, after 3 MRT trips), Professor Dame N. Seah has no umbrella left in her home?  

(iv) Without explicitly solving, can you find out the steady state probabilities for this Markov chain?  
*(10 Marks)*

---

### 关键条件复述（中文）

**3(a)**  
- 系统输入噪声 \(x(t)\) 是实 WSS 白噪声，自相关 \(R_{xx}(t_1,t_2) = 5\delta(t_1-t_2)\)。  
- 放大器增益在 \(t=0\) 时从 1 增加到 100，在 \(t=2\) 时降回 1。  
- 输出过程：  
\[
y(t) = \begin{cases} 100x(t), & 0 \leq t \leq 2 \\ x(t), & \text{其他} \end{cases}
\]  
- 求 \(R_{yy}(t_1,t_2)\) 分三种情况：  
  - (i) \(t_1, t_2 \in [0,2]\)  
  - (ii) 一个在 \([0,2]\) 内，另一个在外  
  - (iii) 两个都在 \([0,2]\) 外  
- 判断 \(y(t)\) 是否 WSS（是否只依赖于 \(t_1-t_2\)）？是否白噪声（是否形如 \(q(t_1)\delta(t_1-t_2)\)）？

**3(b)**  
- 公交车到达数 \(w(t)\) 是泊松过程，\(E[w(5)] = 1 \Rightarrow \lambda = 1/5\)。  
- 至少 2 辆车到才能上车，4 辆保证能上。  
- (i) 求 10 分钟内到达 2 到 4 辆的概率 \(P(2 \leq w(10) \leq 4)\)。  
- (ii) 求 \(w(10)\) 的方差。

**3(c)**  
- 离散时间白噪声 \(x[n]\)，功率谱 \(S_{xx}(\omega) = 2\)。  
- 通过系统 \(H(z) = 1/(1 - 0.5z^{-1})\) 得到 AR(1) 过程 \(y[n]\)。  
- 求 \(S_{yy}(\omega)\) 并证明它是实函数。

**4(a)**  
- 实平稳零均值过程 \(x(t)\)，自协方差 \(C_{xx}(\tau) = e^{-|\tau|}\)。  
- (i) 判断 \(x(t)\) 是否均值遍历（用 Slutsky 定理）。  
- (ii) 已知四阶矩  
\[
E[x(t+\lambda+\tau)x(t+\tau)x(t+\lambda)x(t)] = e^{-2|\lambda|}g(\tau)
\]  
其中  
\[
g(\tau) = \begin{cases} 3 - |\tau|, & |\tau|<1 \\ (|\tau|+1)/|\tau|, & |\tau| \geq 1 \end{cases}
\]  
判断 \(x(t)\) 是否协方差遍历（定义 \(z(t)\) 并用 Slutsky 定理）。

**4(b)**  
- Professor Seah 在家有 3 把伞。  
- 每天早晨下雨概率 0.2。若下雨且家有伞，则带一把伞并忘在 MRT。  
- (i) 建立马尔可夫链，状态 = 早晨出发前家里的伞数（状态 0 为吸收态）。画图并标转移概率。  
- (ii) 求转移矩阵 \(\Pi[1]\)。  
- (iii) 已知周一早晨从状态 3 开始，求周四早晨状态为 0（无伞）的概率。  
- (iv) 不显式求解，能否判断稳态概率？





**2023** 







### 

**1. (a)**  
Suppose \( X \) is selected uniformly at random from the interval \([-1, 1]\). Define the events  
\[
A = \{X < 0\}, \quad B = \{|X - 0.5| < 1\}, \quad \text{and} \quad C = \{X > 0.75\}.
\]  
Find the probabilities of  
(i) \( A \cap B \),  
(ii) \( A \cap C \),  
(iii) \( A \cup B \), and  
(iv) \( A \cup C \).  

**(b)**  
Let \( A \) be the event that a patient develops long COVID symptoms and \( B \) be the event that the patient is unvaccinated. A study has found that if a patient is unvaccinated, he or she is more likely to develop long COVID symptoms, i.e., \(\mathbb{P}(A | B) \geq \mathbb{P}(A)\). Given a vaccinated patient, what can you say about the conditional probability of the patient developing long COVID symptoms? Justify your answer rigorously.  

*(7 Marks)*

**(c)**  
Let \( X \sim \text{Exp}(\lambda) \) be an exponential random variable with parameter \(\lambda\) and \( Y = \lfloor X \rfloor \) be the integer part of \( X \), i.e., \( Y = k \) for \( k \leq X < k + 1, k = 0, 1, \ldots \).  
(i) Find the pmf of \( Y \).  
(ii) Let \( Z = X - Y \) be the quantization error. Find the pdf of \( Z \).  

*(12 Marks)*

**2. (a)**  
Consider the noisy channel shown in Figure 1, where \( X \) and \( Z \) are independent, and \( a \) and \( b \) are constants.  

\[
Z \sim \mathcal{N}(0, N)
\]  

\[
X \sim \mathcal{N}(0, P) \xrightarrow{\times a} \oplus \xrightarrow{\times b} Y = b(aX + Z)
\]  

**Figure 1**  

(i) Find the mean and variance of \( Y \).  
(ii) Find the covariance between \( X \) and \( Y \).  
(iii) Are the minimum mean square error (MMSE) estimate of \( X \) given \( Y \) and its MMSE linear estimate the same? Why or why not? Find the MMSE linear estimate of \( X \) given \( Y \) and its MSE.  

*(20 Marks)*

**(b)**  
Suppose \( X_1, X_2, \ldots \) are i.i.d. random variables, each with pdf \( f(x) = \lambda e^{-\lambda x} \) for \( x \geq 0 \). Let \( Y_n = \min\{X_1, X_2, \ldots, X_n\} \). Show that \( Y_n \) converges to 0 in probability as \( n \to \infty \).  

*(5 Marks)*

---

### 关键条件复述（中文）

**1(a)**  
- \(X\) 在区间 \([-1,1]\) 上均匀分布。  
- 事件定义：  
  - \(A = \{X < 0\}\)  
  - \(B = \{|X - 0.5| < 1\}\)  
  - \(C = \{X > 0.75\}\)  
- 求概率：  
  - (i) \(A \cap B\)  
  - (ii) \(A \cap C\)  
  - (iii) \(A \cup B\)  
  - (iv) \(A \cup C\)

**1(b)**  
- \(A\)：患者出现长新冠症状  
- \(B\)：患者未接种疫苗  
- 已知 \(\mathbb{P}(A|B) \geq \mathbb{P}(A)\)  
- 问：给定患者已接种，出现长新冠症状的条件概率如何？需严格证明。

**1(c)**  
- \(X \sim \text{Exp}(\lambda)\)  
- \(Y = \lfloor X \rfloor\)（取整）  
- (i) 求 \(Y\) 的概率质量函数（pmf）  
- (ii) \(Z = X - Y\)（量化误差），求 \(Z\) 的概率密度函数（pdf）

**2(a)**  
- 独立随机变量：\(X \sim \mathcal{N}(0,P)\)，\(Z \sim \mathcal{N}(0,N)\)  
- 系统：\(Y = b(aX + Z)\)，其中 \(a, b\) 为常数  
- 求：  
  - (i) \(Y\) 的均值和方差  
  - (ii) \(X\) 与 \(Y\) 的协方差  
  - (iii) \(X\) 给定 \(Y\) 的 MMSE 估计与 MMSE 线性估计是否相同？为什么？求 MMSE 线性估计及其 MSE

**2(b)**  
- \(X_1, X_2, \ldots\) 独立同分布，pdf 为 \(f(x) = \lambda e^{-\lambda x} (x \geq 0)\)  
- \(Y_n = \min\{X_1, \ldots, X_n\}\)  
- 证明：当 \(n \to \infty\) 时，\(Y_n\) 依概率收敛到 0



### 

**3. (a)**  
_Channelling:_ Entrusted with the task of channelling two real signals, modelled by real jointly wide sense stationary (WSS) random processes \( \mathbf{x}(t) \) and \( \mathbf{y}(t) \), researcher Chan Eh Ling realizes that at the receiver of one signal, the other signal acts as an interference. The auto-correlations \( R_{xx}(\tau) \), \( R_{yy}(\tau) \), and the cross-correlation \( R_{xy}(\tau) \) are available to researcher Chan. Chan Eh Ling compares the magnitude of the cross-correlation of two signals, \( |R_{xy}(\tau)| \), to the average power of both signals, \( \frac{1}{2}[R_{xx}(0)+R_{yy}(0)] \). Without any further information, you should be able to compare \( |R_{xy}(\tau)| \) and \( \frac{1}{2}[R_{xx}(0)+R_{yy}(0)] \). In particular, determine the most appropriate one among the following:  
*(题干不完整，但问题是比较这两个量的大小关系)*

**(b)**  
Continuing the same task, Chan Eh Ling now considers combining two signals into a complex signal, modelled by a complex WSS random process \( \mathbf{w}(t) \) having autocorrelation \( R_{ww}(\tau) \). Chan studies how much the signal \( \mathbf{w}(t) \) changes during a time difference of \(\tau\). This change, in the mean square sense, is given by \( E\{|\mathbf{w}(t+\tau)-\mathbf{w}(t)|^2\} \). Chan feels this change should be compared to the real part of the difference in auto-correlation values, \( \operatorname{Re}[R_{ww}(0)-R_{ww}(\tau)] \).  

Without any further information, you should be able to compare \( E\{|\mathbf{w}(t+\tau)-\mathbf{w}(t)|^2\} \) and \( 2\operatorname{Re}[R_{ww}(0)-R_{ww}(\tau)] \). In particular, determine the most appropriate one among the following:  
*(题干不完整，但问题是比较这两个量的大小关系)*

**(c)**  
_Haze Law:_ With the deteriorating haze situation in Singapore, Ms. Hazel Aw introduces a law against haze. The Pollutant Standards Index (PSI) is modelled as a real stationary white noise process \( \mathbf{w}[n] \) with auto-correlation \( R_{ww}[m] = \delta[m] \). Ms. Aw measures the haze using \( \mathbf{s}[n] \), which is a random process that is obtained by passing \( \mathbf{w}[n] \) through a linear system with transfer function \( H(z) = 1 + \frac{1}{2}z^{-1} \) (Figure 2). Since Hazel Aw uses the auto-correlation of \( \mathbf{s}[n] \) in the proposed law, you’ll help her find the auto-correlation.  

![Image]  
**Figure 2**  

(i) Find \( S_{ss}(\omega) \), the power spectrum of \( \mathbf{s}[n] \). Simplify so that \( S_{ss}(\omega) \) is a real function of \( \omega \).  

(ii) Find \( S_{ss}(z) \), the \( z \)-transform domain power spectrum of \( \mathbf{s}[n] \). [Hint: \( z \)-transform of \( y[n] \) is defined as \( Y(z)=\sum_{n=-\infty}^{\infty}y[n]z^{-n} \). The \( z \)-transform of \( \delta[n-n_{0}] \), an impulse at \( n_{0} \), is therefore \( z^{-n_{0}} \).]  

(iii) Find \( R_{ss}[m] \), the auto-correlation of \( \mathbf{s}[n] \). [Hint: You may use any of the following approaches: the time-domain approach, the inverse Fourier transform approach, or the inverse \( z \)-transform approach.]  
*(9 Marks)*

**(d)**  
Ms. Aw, however, finds that the experimental values of \( \mathbf{s}[n] \) are noisy. The experimental values of the measured haze are given by \( \mathbf{x}[n] = \mathbf{s}[n] + \mathbf{v}[n] \), where \( \mathbf{v}[n] \) is a real stationary white noise (see Figure 3), which is uncorrelated to \( \mathbf{s}[n] \), and has the auto-correlation \( R_{vv}[m] = \frac{7}{8}\delta[m] \). Ms. Aw decides to use a whitening filter to reduce the experimental noise, and needs your help.  

**Figure 3:**  

(i) Find \( S_{xx}(z) \), the \( z \)-transform domain power spectrum of \( \mathbf{x}[n] \).  

(ii) The transfer function of a discrete-time whitening filter \( \Gamma_{x}(z) \) is such that \( S_{xx}(z) = \frac{1}{\Gamma_{x}(z) \Gamma_{x}(z^{-1})} \). Find the whitening filter \( \Gamma_{x}(z) \) by factorizing the \( z \)-transform domain power spectrum \( S_{xx}(z) \).  
*(9 Marks)*

---

### 关键条件复述（中文）

**3(a)**  
- 两个实联合 WSS 过程 \( \mathbf{x}(t) \), \( \mathbf{y}(t) \)，已知 \( R_{xx}(\tau) \), \( R_{yy}(\tau) \), \( R_{xy}(\tau) \)。  
- 比较 \( |R_{xy}(\tau)| \) 与 \( \frac{1}{2}[R_{xx}(0)+R_{yy}(0)] \) 的大小关系。

**3(b)**  
- 复 WSS 过程 \( \mathbf{w}(t) \)，自相关 \( R_{ww}(\tau) \)。  
- 比较 \( E\{|\mathbf{w}(t+\tau)-\mathbf{w}(t)|^2\} \) 与 \( 2\operatorname{Re}[R_{ww}(0)-R_{ww}(\tau)] \) 的大小关系。

**3(c)**  
- 实平稳离散白噪声 \( \mathbf{w}[n] \)，自相关 \( R_{ww}[m] = \delta[m] \)。  
- 通过系统 \( H(z) = 1 + \frac{1}{2}z^{-1} \) 得到 \( \mathbf{s}[n] \)。  
- 求：  
  - (i) \( S_{ss}(\omega) \)（功率谱，需化为实函数）  
  - (ii) \( S_{ss}(z) \)（z 变换域功率谱）  
  - (iii) \( R_{ss}[m] \)（自相关函数）

**3(d)**  
- 观测信号 \( \mathbf{x}[n] = \mathbf{s}[n] + \mathbf{v}[n] \)，其中 \( \mathbf{v}[n] \) 是实平稳白噪声，与 \( \mathbf{s}[n] \) 不相关，且 \( R_{vv}[m] = \frac{7}{8}\delta[m] \)。  
- 求：  
  - (i) \( S_{xx}(z) \)（\( \mathbf{x}[n] \) 的 z 变换域功率谱）  
  - (ii) 白化滤波器 \( \Gamma_{x}(z) \)，满足 \( S_{xx}(z) = \frac{1}{\Gamma_{x}(z) \Gamma_{x}(z^{-1})} \)，通过谱分解求得。

### 

**4. (a)**  
_Addiction:_ Mr. A. Dickson has lots of money, and has an addiction to gambling. He decides to play non-stop until he hits the jackpot of one million dollars. Denote the time the jackpot is won by a random variable **c**. From the published odds, Mr. A. Dickson figures that winning of the jackpot is equally likely to happen anytime during the next 500 days. Therefore **c** has uniform density in \(0 \leq t \leq 500\) where time \(t\) is measured in days. Let a process \(x(t) = 10^6\delta(t - c)\) represents Mr. A. Dickson’s gain in dollars when he hits the jackpot. However, playing for the jackpot costs him $3000 a day. Let another process \(y(t) = -3000\{U(t) - U(t - c)\}\) represents his cost in dollars, where \(U(t)\) denotes the unit step function, and the negative amplitude denotes loss of money.

(i) In this part, find \(R_{xx}(t_1, t_2)\), the auto-correlation of the winning process. [Hint: \(x(t)\) is a non-stationary process. \(\int_p^q \delta(t_1 - c)\delta(t_2 - c)dc = \delta(t_1 - t_2)\) if both \(t_1\) and \(t_2\) are inside the interval \([p, q]\), but \(= 0\) otherwise.]

(ii) In this part, we find the expectation of \( x(t) + y(t) \), the expected gain or loss of Mr. A. Dickson. First, show that the expectation of the winning process \( x(t) \) is given by

\[E\{x(t)\} = 
\begin{cases} 
2000 & 0 \leq t \leq 500 \\
0 & \text{otherwise}
\end{cases}\]

which confirms that the expected winning does not change over time since \( c \) is uniform. [Hint: \(\int_{p}^{q} \delta (t - c) dc = 1\) if \( t \) is inside the interval \([p, q]\), but \( = 0 \) if \( t \) is outside this interval.]

(iii) Second, find \( E\{y(t)\} \), the expectation of the cost process \( y(t) \). [Hint: \(\int_{p}^{q} U(t - c) dc = \int_{p}^{q} dc\) if \( q < t \), \( = \int_{p}^{t} dc\) if \( t \) is inside the interval \([p, q]\), and \( = 0 \) if \( t < p \). The expected cost \( E\{y(t)\} \) should be negative since cost is negative. It should be a function of time, and it should approach 0 over time, since Mr. A. Dickson stops playing as soon as he wins, and his win becomes more and more likely as time passes.]

*(14 Marks)*

**(b)**  
*Reign of a Queen*: In a faraway country called United Queendom (UQ), a Queen reigns for as long as she lives. Let \( a_i \) denote the \( i \)-th year of the reign of the Queen. For simplicity, assume that \( 1 \leq i \leq \infty \).

- With probability \( p \), the Queen does not survive the \( i \)-th year, and a new Queen is coronated such that the reign of the (new) Queen restarts at \( a_1 \).
- Otherwise, the Queen lives through the \( i \)-th year, and her reign then extends to \( a_{i+1} \).

(i) Formulate the above problem as a discrete-time Markov chain with infinite number of states. Draw the Markov chain, showing a few states and transition probabilities. Find the state transition matrix.

(ii) Find the steady state probabilities. What is the probability that any Queen of UQ reigns for more than 70 years?

*(题干不完整，但问题如上)*

---

### 关键条件复述（中文）

**4(a)**  
- 随机变量 \(c\) 在 \([0, 500]\) 天均匀分布，表示中奖时间。  
- 中奖收益过程：\(x(t) = 10^6 \delta(t - c)\)  
- 每天成本 3000 美元，成本过程：\(y(t) = -3000[U(t) - U(t-c)]\)  
- 求：  
  - (i) \(R_{xx}(t_1, t_2)\)（中奖过程的自相关函数）  
  - (ii) 证明 \(E\{x(t)\} = \begin{cases} 2000 & 0 \leq t \leq 500 \\ 0 & \text{其他} \end{cases}\)  
  - (iii) 求 \(E\{y(t)\}\)（成本过程的期望）

**4(b)**  
- 某国女王统治年份记为 \(a_i\)（第 \(i\) 年）。  
- 每年：  
  - 以概率 \(p\)，女王在第 \(i\) 年去世，新女王继位（状态回到 \(a_1\)）  
  - 以概率 \(1-p\)，女王活过第 \(i\) 年，进入 \(a_{i+1}\)  
- 要求：  
  - (i) 建立无限状态离散时间马尔可夫链，画出示意图，给出转移矩阵  
  - (ii) 求稳态概率，以及任一女王统治超过 70 年的概率







**2022**



### 

**1.**  
Two discrete random variables \( X \) and \( Y \) have possible values of 4, 5 and 6. Table 1 specifies one of their probability-mass functions (PMFs): \( p_{X,Y}(x,y) \), \( p_{Y|X}(y|x) \) or \( p_{X|Y}(x|y) \). Another PMF is specified by Table 2.

**Table 1**

| \( y \) \ \( x \) | 4       | 5       | 6       |
| ----------------- | ------- | ------- | ------- |
| 4                 | \( a \) | 0.1     | 0.5     |
| 5                 | 0.2     | \( b \) | 0.4     |
| 6                 | 0.3     | 0.2     | \( c \) |

**Table 2**

| 4    | 5    | 6       |
| ---- | ---- | ------- |
| 0.3  | 0.4  | \( d \) |

**(a)** Give the conditions (values of \( a, b, \), and \( c \)), under which the Table 1 specifies PMFs, \( p_{Y|X}(y|x) \), \( p_{X|Y}(x|y) \) and \( p_{X,Y}(x,y) \), respectively.

**(b)** If Table 2 (on page 1) specifies \( p_Y(y) \) and Table 1 (on page 1) and Table 2 together fully specify the two random variables \( X \), and \( Y \), what is the value of \( d \) and what PMF is specified by Table 1?  
*(4 Marks)*

**(c)** Under the conditions of 1 (b), produce 3 tables to specify the other 3 PMFs.  
*(10 Marks)*

**2.**  
Two continuous random variables \( X \) and \( Y \) have joint probability density function (pdf)  
\[
p_{X,Y}(x,y) = \lambda y^2 e^{-xy}, \quad x \geq 0, \quad 1 \leq y \leq 5,
\]  
where \( \lambda \) is a constant.

**(a)** Express the minimal mean square error estimation of \( X \) as a function of the random variable \( Y \). If we observed that \( Y=2 \), what is the estimate of \( X \) that has the minimal mean square error?  
*(12 Marks)*

**(b)** For unknown value of \( X \), find the estimate of \( Y \) that has the minimal mean square error. What is the mean square error of the estimate?  
*(题干不完整，但问题如上)*

**3. (a)**  
Suppose the probability of the head showing up is \( p \) in flipping a coin.

(i) You flip the coin until the head shows up. Assuming independent coin flips, derive the probability that you need to flip the coin \( m \) times.  
*(4 Marks)*

(ii) You flip the coin until the head shows up twice. Assuming independent coin flips, derive the probability that you need to flip the coin \( n \) times.  
*(6 Marks)*

**(b)**  
\( x(t) \) is a wide sense stationary (WSS) real random process with mean \( E\{x(t)\} = \mu \) and autocorrelation \( R_{xx}(\tau) = e^{-|\tau|} \). Another process is defined as \( y(t) = x(t) + 2 \).

(i) Find \( E\{y(t)\} \), the mean of \( y(t) \).  
(ii) Find \( R_{yy}(\tau) \), the autocorrelation of \( y(t) \).  
(iii) Is it possible that \( R_{xx}(\tau) = R_{yy}(\tau) \)? If yes, find the required condition for both autocorrelations to be equal.  
*(题干不完整，但问题如上)*

---

### 关键条件复述（中文）

**1**  
- 离散随机变量 \(X, Y\) 取值 {4,5,6}。  
- 表 1 给出某个 PMF（可能是联合、条件 X|Y、条件 Y|X）。  
- 表 2 给出另一个 PMF（可能是边缘分布）。  
- (a) 求 \(a,b,c\) 的值，使得表 1 分别表示 \(p_{Y|X}(y|x)\)、\(p_{X|Y}(x|y)\)、\(p_{X,Y}(x,y)\)。  
- (b) 若表 2 是 \(p_Y(y)\)，且两表共同完全确定 \(X,Y\)，求 \(d\) 并判断表 1 是哪种 PMF。  
- (c) 在 (b) 条件下，用 3 个表格给出另外 3 个 PMF。

**2**  
- 连续随机变量 \(X, Y\) 的联合 pdf：  
\[
p_{X,Y}(x,y) = \lambda y^2 e^{-xy}, \quad x \geq 0, \ 1 \leq y \leq 5
\]  
- (a) 求 \(X\) 基于 \(Y\) 的最小均方误差估计（作为 \(Y\) 的函数）。若观测到 \(Y=2\)，求 \(X\) 的 MMSE 估计。  
- (b) 对未知的 \(X\)，求 \(Y\) 的最小均方误差估计及其 MSE。

**3(a)**  
- 抛硬币正面概率 \(p\)。  
- (i) 一直抛直到出现正面，求需要抛 \(m\) 次的概率。  
- (ii) 一直抛直到出现两次正面，求需要抛 \(n\) 次的概率。

**3(b)**  
- 实 WSS 过程 \(x(t)\)，均值 \(E[x(t)]=\mu\)，自相关 \(R_{xx}(\tau)=e^{-|\tau|}\)。  
- 定义 \(y(t) = x(t) + 2\)。  
- 求：  
  - (i) \(E[y(t)]\)  
  - (ii) \(R_{yy}(\tau)\)  
  - (iii) 是否可能 \(R_{xx}(\tau)=R_{yy}(\tau)\)？若可能，需满足什么条件？







### 

**4. (a)**  
_Fully vaccinated:_ Assume that all 7,000,000,000 persons will become fully vaccinated at a random time \( t \), where \( t \) is uniform between time \( t = 0 \) years and time \( t = 3 \) years. Let a random process \( x(t) \) model the fully vaccinated world as  
\( x(t) = 7,000,000,000 \, U(t - t) \), where \( U(t) \) is the unit step function that is 0 for \( t < 0 \), and is 1 for \( t \geq 0 \).

(i) Determine \( E\{x(t)\} \), the possibility of full vaccination, for all time \( t \). Note that \( x(t) \) is non-stationary.

(ii) Impact of full vaccination on the pandemic is exponential rather that linear. Assume that the impact of the possibility of full vaccination is \( a[x(t)]^b \) for some constants \( a, b \). Determine \( E\{a[x(t)]^b\} \), the expected impact of full vaccination, for all time \( t \).  
*(10 Marks)*

**(b)**  
_A mosquito sensor:_ A sensor triggers an oscillator as soon as a mosquito lands on it. The oscillator having an output \( p + \cos(qt) \) produces an audible tone for a duration of \( 20\pi / q \). Its inventor, Amos Skittow, vouches that mosquito arrivals are Poisson arrivals with \( \lambda \) mosquitoes arriving per unit time. Thus, Mr. Skittow confirms that the oscillator output \( s(t) \) is a shot noise observed at the output of a linear system having the following impulse response:  
\[
h(t) = 
\begin{cases} 
p + \cos(qt) & 0 \leq t \leq 20\pi / q \\ 
0 & \text{elsewhere} 
\end{cases}
\]

(i) Determine \( E\{s(t)\} \), the mean output from Amos Skittow’s oscillator.

(ii) Determine the expected power requirement of the oscillator, or the variance of \( s(t) \), given by  
\[
\sigma_s^2 = R_{ss}(0) - E^2\{s(t)\}.
\]  
[Hint: For a shot noise, \( R_{ss}(\tau) = \lambda^2 H^2(0) + \lambda h(\tau) * h(-\tau) \) where \( H(0) \) may be found from the frequency response \( H(\omega) = \int_{-\infty}^{\infty} h(t)e^{-j\omega t}dt \), and \(*\) means convolution,  
\[
f(t) * g(t) = \int_{-\infty}^{\infty} f(t - \alpha)h(\alpha)d\alpha.
\]  
*(题干不完整，但问题如上)*

**5. (a)**  
A continuous-time homogeneous Markov chain has 2 states and the following transition probability matrix,  
\[
\Pi(\tau) = 
\begin{bmatrix}
0.6 + 0.4e^{-\tau} & ? \\
? & 0.6 + 0.6e^{-\tau}
\end{bmatrix}
\]  
where \( \tau = t_2 - t_1 \) is the time difference.

(i) Find both missing entries in the above transition probability matrix.

(ii) Find the transition probability rate matrix \( \Pi'(0^+) \) for this Markov chain.

(iii) If the state probability vector at time \( t = 0 \) is \( P(0) = [1 \quad 0] \), then find the state probability vector at time \( t = 0.693 \).  
*(8 Marks)*

**(b)**  
_Old problem, young solution:_ Prof. Oldman asked his student Eve R. Young to design a detector based on integrating the received signal from 0 to \( T \) and thresholding. Let \( s(t) \) be the received signal which is real, WSS, and let \( R_{ss}(\tau) \) be its autocorrelation. Its desired integral is a random variable \( z = \int_0^T s(t)dt \). Rather than designing an integrator circuit, Ms. Eve R. Young built a simpler circuit using value(s) of \( s(t) \) to estimate \( z \).

(i) Using just one value of \( s(t) \), Eve R. Young guessed the middle value would be the best choice, and designed an estimator as \( \hat{z} = a s(T/2) \) (estimator-1). Show that the optimal MS estimator-1 has \( a = \frac{2}{R_{ss}(0)} \int_0^{T/2} R_{ss}(x)dx \).

(ii) Prof. Oldman was not happy with the estimator-1 performance, so Eve R. Young decided to improve the estimation by using two extreme values, or \( \hat{z} = b s(0) + c s(T) \) (estimator-2). Find the values of \( b \) and \( c \) in terms of \( R_{ss}(\tau) \) for the optimal MS estimator-2. (For typical autocorrelation functions, the LMS error of estimator-2 is indeed smaller than estimator-1, making the professor happy.)

(iii) Over dinner, Eve R. Young’s friend told her to use the average value obtained from both extremes, or \( \hat{z} = d \cdot \frac{s(0)+s(T)}{2} \) (estimator-3). Without solving \( d \) but using your solution of estimator-2, comment on whether estimator-3 performs better than, same as, or worse than estimator-2.  
*(题干不完整，但问题如上)*

---

### 关键条件复述（中文）

**4(a)**  
- 全球 70 亿人，每个人在 [0,3] 年内均匀随机时间完成疫苗接种。  
- 过程 \(x(t) = 7\times 10^9 \cdot U(t - t)\)（此处应为 \(U(t - \text{随机时间})\)，原题似有笔误）。  
- (i) 求 \(E[x(t)]\)（所有时间 t）。  
- (ii) 疫苗接种影响为 \(a[x(t)]^b\)，求 \(E\{a[x(t)]^b\}\)。

**4(b)**  
- 蚊子到达为泊松过程，速率 \(\lambda\)。  
- 传感器触发振荡器，输出 \(p + \cos(qt)\)，持续 \(20\pi/q\)。  
- 系统冲激响应 \(h(t) = p + \cos(qt)\)（当 \(0 \leq t \leq 20\pi/q\)），否则 0。  
- (i) 求 \(E[s(t)]\)（输出均值）。  
- (ii) 求输出方差 \(\sigma_s^2 = R_{ss}(0) - E^2[s(t)]\)。  
- 提示：散粒噪声自相关公式给出。

**5(a)**  
- 连续时间齐次马尔可夫链，2 状态，转移概率矩阵：  
\[
\Pi(\tau) = 
\begin{bmatrix}
0.6 + 0.4e^{-\tau} & ? \\
? & 0.6 + 0.6e^{-\tau}
\end{bmatrix}
\]  
- (i) 求缺失的两个元素。  
- (ii) 求转移概率率矩阵 \(\Pi'(0^+)\)。  
- (iii) 若初始状态概率向量 \(P(0) = [1, 0]\)，求 \(t=0.693\) 时的状态概率向量。

**5(b)**  
- 实 WSS 信号 \(s(t)\)，自相关 \(R_{ss}(\tau)\)。  
- 需要估计 \(z = \int_0^T s(t) dt\)。  
- (i) 估计器1：\(\hat{z} = a s(T/2)\)，证明最优 \(a = \frac{2}{R_{ss}(0)} \int_0^{T/2} R_{ss}(x)dx\)。  
- (ii) 估计器2：\(\hat{z} = b s(0) + c s(T)\)，求最优 \(b, c\)（用 \(R_{ss}(\tau)\) 表示）。  
- (iii) 估计器3：\(\hat{z} = d \cdot \frac{s(0)+s(T)}{2}\)，不计算 \(d\)，仅根据估计器2的结果评论性能比较。







**2021**

### 

**1.**  
A random variable \( X \) is specified by its probability density function (pdf)

\[
f_X(x) = 
\begin{cases} 
a(1 - 0.1x), & 0 \leq x \leq 10 \\
0, & \text{otherwise}
\end{cases}
\]

Five numbers drawn from \( X \) are \( x_1 = 0.3, \, x_2 = 1, \, x_3 = 2.5, \, x_4 = 4.5 \) and \( x_5 = 7 \).

**(a)** From the 5 random numbers \( x_k \), generate 5 random numbers \( y_k \) that obey the uniform distribution from zero to one.  
*(12 Marks)*

**(b)** From the 5 random numbers \( x_k \), generate 5 random numbers \( z_k \) that obey the distribution specified by the pdf

\[
f_z(z) =
\begin{cases} 
bz, & 0 \leq z \leq 10 \\
0, & \text{otherwise}
\end{cases}
\]  
*(13 Marks)*

**2.**  
A random variable \( X \) has the probability mass function (pmf) \( p_X(0) = 0.4 \) and \( p_X(2) = 0.6 \). The conditional probability density function (pdf) \( f_{Y|X}(y|x) \) of a random variable \( Y \) is given by

\[
f_{Y|X}(y|0) =
\begin{cases} 
b_1 y & 0 \leq y \leq 4 \\
0 & \text{otherwise}
\end{cases}
\]

\[
f_{Y|X}(y|2) =
\begin{cases} 
b_2 (4 - y) & 0 \leq y \leq 4 \\
0 & \text{otherwise}
\end{cases}
\]

It is observed that \( y = 2.5 \).

**(a)** Estimate the value of \( X \) to achieve the lowest probability of the wrong estimation.  
*(13 Marks)*

**(b)** Estimate the value of \( X \) to have the minimal mean square error of the estimation.  
*(12 Marks)*

**3.**  
*Spread of the pandemic*: Komal Vidyarthi, an NTU researcher who is lovingly called Ko. Vid. by her friends, uses the following exponential model to study the spread of a pandemic in a community. The percentage of infected people is a real random variable \( x \) having uniform density \( f_x(x) \) from 0 to 10. The number of people who are at a risk of infection at time \( t \geq 0 \) is a real non-stationary random process \( y(t) = e^{xt} \).

**(a)** Komal wishes to find the first order statistics of \( y(t) \). In the first step, find \( \eta_y(t) \), the mean of \( y(t) \), for \( t \geq 0 \).  
*(6 Marks)*

**(b)** In the second step, using \( f_x(x) \), the density of \( x \), find \( f_y(y,t) \), the first order density of \( y(t) \), for \( t \geq 0 \).  
*(10 Marks)*

**(c)** Ko. Vid. found that \( y(t) \) has a strange property. The second order statistics of \( y(t) \) may be found from its first order statistics. Express \( R_{yy}(t_1, t_2) \), the autocorrelation of \( y(t) \), in terms of \( \eta_y(t) \), the mean of \( y(t) \), for \( t_1, t_2 \geq 0 \).  
*(5 Marks)*

**(d)** Combining your results of parts (a) and (c), find \( R_{yy}(t_1, t_2) \) for \( t_1, t_2 \geq 0 \).  
*(4 Marks)*

---

### 关键条件复述（中文）

**1**  
- 随机变量 \(X\) 的 pdf：  
\[
f_X(x) = a(1 - 0.1x), \quad 0 \leq x \leq 10
\]  
- 已知 5 个样本：\(x_1=0.3, x_2=1, x_3=2.5, x_4=4.5, x_5=7\)  
- (a) 用这 5 个样本生成 5 个服从 [0,1] 均匀分布的随机数 \(y_k\)  
- (b) 用这 5 个样本生成 5 个服从 pdf \(f_z(z) = b z \ (0 \leq z \leq 10)\) 的随机数 \(z_k\)

**2**  
- \(X\) 的 pmf：\(p_X(0)=0.4, p_X(2)=0.6\)  
- 条件 pdf：  
  - \(f_{Y|X}(y|0) = b_1 y, \ 0 \leq y \leq 4\)  
  - \(f_{Y|X}(y|2) = b_2 (4-y), \ 0 \leq y \leq 4\)  
- 观测到 \(y=2.5\)  
- (a) 以最小错误概率估计 \(X\)  
- (b) 以最小均方误差估计 \(X\)

**3**  
- 感染百分比 \(x\) 在 [0,10] 上均匀分布  
- 风险人数过程：\(y(t) = e^{x t}, \ t \geq 0\)  
- (a) 求均值 \(\eta_y(t) = E[y(t)]\)  
- (b) 求一阶密度 \(f_y(y,t)\)  
- (c) 用均值 \(\eta_y(t)\) 表示自相关 \(R_{yy}(t_1,t_2)\)  
- (d) 结合 (a)(c) 求 \(R_{yy}(t_1,t_2)\)





### 

**4. (a)**  
Let \( x[n] \) be a discrete time real stationary random process with autocorrelation

\[
R_{xx}[m] = 
\begin{cases} 
2 & m = 0 \\
1 & m = -1,1 \\
0 & \text{else} 
\end{cases}
\]

Let \( y[n] = 2x[n] - x[n-1] \) be another random process. Note that \( y[n] \) is the output process when the input process \( x[n] \) passes through a linear system with impulse response

\[
h[n] = 
\begin{cases} 
2 & n = 0 \\
-1 & n = 1 \\
0 & \text{else} 
\end{cases}
\]

(i) Find \( S_{xx}(\omega) \), the power spectrum of \( x[n] \). Also find \( S_{xx}(z) \), the z-transform-domain power spectrum of \( x[n] \).

(ii) Find \( R_{yy}[m] \), the autocorrelation of \( y[n] \).

(iii) Find \( S_{yy}(\omega) \), the power spectrum of \( y[n] \). Also find \( S_{yy}(z) \), the z-transform-domain power spectrum of \( y[n] \).

**(b)**  
PCR (polymerase chain reaction) test: Everyone in Jurong Technological University is PCR tested each week, with one of three possible outcomes: negative, (positive and) asymptomatic, or (positive and) symptomatic. The following facts are observed.

- An asymptomatic person cannot become symptomatic next week. Similarly, a symptomatic person cannot become asymptomatic next week.
- Without any medical treatment, recovery of an asymptomatic person is slow. The probability that an asymptomatic person becomes negative next week is observed to be \( M \) times higher than the probability that a negative person becomes asymptomatic next week. The value of \( M \) is observed to be 2.
- With medical treatment, recovery of a symptomatic person is fast. As a result, the probability that a symptomatic person becomes negative next week is \( N \) times higher than the probability that a negative person becomes symptomatic next week. The value of \( N \) is observed to be 4.

(i) Formulate the above problem as a discrete-time Markov chain (with unit of time being week), where the states are negative, asymptomatic, and symptomatic. Draw the Markov chain and find the transition matrix. If the actual transition probabilities are not specified above, you may use variables.

(ii) Find the steady state probabilities. If the population of the Jurong Technological University is 35000, how many people are symptomatic on an average in the steady state? [Hint: You should be able to evaluate the steady state probabilities in spite of any variable you may have used in part (b)(i).]

(iii) With improved medical treatment, it is possible to achieve faster recovery and, therefore, lesser number of symptomatic people. Find the condition on \( N \) such that the number of symptomatic people on an average does not exceed 3500 in the steady state.

*(11 Marks)*

---

### 关键条件复述（中文）

**4(a)**  
- 实平稳离散时间过程 \(x[n]\)，自相关：  
\[
R_{xx}[m] = 
\begin{cases} 
2, & m=0 \\ 
1, & m=\pm 1 \\ 
0, & \text{其他}
\end{cases}
\]  
- 输出过程：\(y[n] = 2x[n] - x[n-1]\)，系统冲激响应 \(h[n] = \{2, -1\}\)（在 n=0,1）  
- 求：  
  - (i) \(S_{xx}(\omega)\) 和 \(S_{xx}(z)\)  
  - (ii) \(R_{yy}[m]\)  
  - (iii) \(S_{yy}(\omega)\) 和 \(S_{yy}(z)\)

**4(b)**  
- 每周 PCR 测试结果状态：阴性(Neg)、无症状(Asym)、有症状(Sym)  
- 状态转移限制：Asym ⇄ Sym 不可能  
- 恢复概率关系：  
  - Asym → Neg 的概率 = \(M \times\) (Neg → Asym 的概率)，\(M=2\)  
  - Sym → Neg 的概率 = \(N \times\) (Neg → Sym 的概率)，\(N=4\)  
- (i) 建立三状态离散时间马尔可夫链，画图，求转移矩阵（可用变量）  
- (ii) 求稳态概率；若总人口 35000，稳态下平均有症状人数  
- (iii) 求 \(N\) 满足什么条件时，稳态平均有症状人数不超过 3500





**2020**

### 

**1.**  
Two random variables \( X \) and \( Y \) are specified by their joint probability density function (pdf)

\[
f(x, y) = 
\begin{cases} 
cxy & x \geq 0, y \geq 0, x + y \leq 1 \\
0 & \text{otherwise}
\end{cases}
\]

**(a)** Find the marginal pdf \( f_Y(y) \).  
*(5 Marks)*

**(b)** Find the conditional pdf \( f_{X|Y}(x | y) \).  
*(5 Marks)*

**(c)** Estimate the value of \( X \) based on the observed value of \( Y = y \) so that the mean square error (MSE) is minimized.  
*(5 Marks)*

**(d)** Compute the MSE for a given observed value \( Y = y \).  
*(5 Marks)*

**2.**  
Table 1 completely specifies two discrete random variables \( X \) and \( Y \).

**Table 1**

| \( y \) \ \( x \) | 4    | 5    | 6    |
| ----------------- | ---- | ---- | ---- |
| 1                 | 0    | 0.15 | 0.15 |
| 3                 | 0.08 | 0.08 | 0.24 |
| 7                 | 0.09 | 0.18 | 0.03 |

**(a)** Does Table 1 specify the probability mass function (PMF) \( p_{X,Y}(x, y) \), \( p_{Y|X}(y|x) \), or \( p_{X|Y}(x|y) \)? Give the reasons for your answer.  
*(6 Marks)*

**(b)** What PMF (\( p_{Y}(y) \)) is specified by the 3 numbers (0.08, 0.08, 0.24) drawn from the second row of Table 1?  
*(2 Marks)*

**(c)** If we normalize the above 3 numbers by the sum of them, i.e., (0.08, 0.08, 0.24) / (0.08+0.08+0.24), what PMF (\( p_{X|Y}(x|y) \)) is specified by the results? Give the reasons for your answer.  
*(6 Marks)*

**(d)** If we divide the 3 numbers (0.08, 0.08, 0.24), respectively by the sum of the numbers in the corresponding column of Table 1, what PMF (\( p_{Y|X}(y|x) \)) is specified by the results? Give the reasons for your answer.  
*(6 Marks)*

**3. (a)**  
A 2-digit integer \( x \), \( 10 \leq x \leq 99 \), is randomly chosen. All possible choices are equally likely.

(i) What is the probability of event \( A \) that the ones-digit of \( x \) has the maximum value and what is the probability of event \( B \) that the tens-digit of \( x \) has the maximum value?

(ii) What is the probability of event \( C \) that at least one digit of \( x \) has the maximum value?  
*(10 Marks)*

**(b)**  
\( x[n] \) is a real wide-sense stationary (WSS) discrete-time random process with autocorrelation \( R_{xx}[m] = 2e^{-0.5|m|} \). Let \( y[n] = x[n] - x[n-3] \).

(i) Find \( \eta_y[n] = E\{y[n]\} \), the mean of \( y[n] \).

(ii) Find \( E\{y^2[n]\} \), the average power of \( y[n] \).

(iii) Find \( R_{yy}[m] \), the autocorrelation of \( y[n] \). Hence, show that for \( |m| \geq 3 \), it may be simplified to \( R_{yy}[m] = cR_{xx}[m] \), where \( c \) is a constant. Find \( c \).  
*(10 Marks)*

---

### 关键条件复述（中文）

**1**  
- 联合 pdf：\( f(x,y) = cxy \)，定义域 \( x \geq 0, y \geq 0, x+y \leq 1 \)  
- (a) 求边缘 pdf \( f_Y(y) \)  
- (b) 求条件 pdf \( f_{X|Y}(x|y) \)  
- (c) 基于观测 \( Y=y \)，求最小 MSE 的 \( X \) 估计  
- (d) 对给定 \( Y=y \)，计算 MSE

**2**  
- 表 1 给出 \( X \)（取值 4,5,6）和 \( Y \)（取值 1,3,7）的联合分布  
- (a) 判断表 1 是联合 PMF \( p_{X,Y} \)、条件 PMF \( p_{Y|X} \)、还是 \( p_{X|Y} \)？说明理由  
- (b) 第二行三个数 (0.08, 0.08, 0.24) 表示什么 PMF？  
- (c) 将这三个数归一化（除以它们的和）后表示什么 PMF？说明理由  
- (d) 将这三个数分别除以对应列的和，表示什么 PMF？说明理由

**3(a)**  
- 随机选 2 位整数 \( x \in [10,99] \)，等可能  
- (i) 事件 A：个位数字最大；事件 B：十位数字最大；求概率  
- (ii) 事件 C：至少一位数字最大；求概率

**3(b)**  
- 实 WSS 离散时间过程 \( x[n] \)，自相关 \( R_{xx}[m] = 2e^{-0.5|m|} \)  
- \( y[n] = x[n] - x[n-3] \)  
- 求：  
  - (i) 均值 \( E[y[n]] \)  
  - (ii) 平均功率 \( E[y^2[n]] \)  
  - (iii) 自相关 \( R_{yy}[m] \)，证明当 \( |m| \geq 3 \) 时 \( R_{yy}[m] = c R_{xx}[m] \)，求常数 \( c \)









### 

**4. (a)**
*Stoopin’ Low:* HK Commissioner of Police Stoophen Lo is accused of stoopin’ low – using police brutality and violence – in his department’s fight against the youth demonstrators. Mr. Lo starts each day with a peaceful mind, but too many demonstrations make him angry. Let x(t)**x**(*t*) = {number of demonstrations starting from time 0 to t, where t is measured in hours} be a Poisson process, such that the probability of k demonstrations is given by P{x(t)=k}=e−λt(λt)k/k!*P*{**x**(*t*)=*k*}=*e*−*λ**t*(*λ**t*)*k*/*k*!. It is known that, on average, there are 6 demonstrations per day, or E{x(24)}=6*E*{**x**(24)}=6.

(i) Find the variance of x(24)**x**(24), the number of demonstrations in a day.

(ii) Mr. Lo spends hour 0 to hour 8 each day in his office, and remains peaceful as long as there are 4 or less demonstrations. He gets agitated if there are 5 to 7 demonstrations. Find the probability that Mr. Lo will be agitated in a day, that is, the probability that there are 5 to 7 demonstrations in 0 to 8 hours, or P{5≤x(8)≤7}*P*{5≤**x**(8)≤7}.

(iii) If the number of demonstrations reaches 8 within his 8 hours in office, it makes Stoophen Lo getting angry and stoopin’ low. Today, it has been 6 hours in office, and so far, 5 demonstrations have taken place, or x(6)=5**x**(6)=5. Find the conditional probability that Stoophen Lo will not be stoopin’ low today, that is, the conditional probability that there will be less than 8 demonstrations in 8 hours, or P{x(8)<8∣x(6)=5}*P*{**x**(8)<8∣**x**(6)=5}.

[Hint: Express the conditional probability as the ratio of a joint probability and a marginal probability. Simplify the joint probability using the fact that non-overlapping Poisson intervals are independent.]
*(12 Marks)*

**(b)**
*Seeing the Doctor:* During an epidemic, Doctor See You Soon from the NTU Health Center classifies each NTU person as healthy, infected (but not sick), or sick.

- The probability that a healthy person becomes infected is p*p*, but a healthy person cannot become sick without getting infected first.
- An infected person may become sick with probability q*q*, or may become healthy with probability p*p*.
- Once a person is sick, he/she sees Doctor See You Soon. After seeing the Doctor, a sick person may become healthy with probability q*q*, while a sick person remains sick and needs to see Doctor See again with a probability 1−q1−*q*. A sick person cannot become infected.

(i) Formulate the above problem as a Markov chain, where the states are healthy, infected, and sick. Draw the Markov chain and find the transition matrix.

(ii) Find the condition on p*p* and q*q* such that 90% or more of NTU people are healthy on an average, that is, the steady state probability Phealthy≥0.9*P*healthy≥0.9.
*(8 Marks)*

**5.**
*Engineering:* To verify the effectiveness of the new air-conditioning system in the School of EEE, Mr. Eng Ine Er placed n*n* temperature sensors randomly in the School. Each sensor output is the difference between the measured temperature and the preset temperature. The i*i*-th sensor output is a real zero mean wide-sense stationary (WSS) random process yi(t)*y**i*​(*t*) with autocorrelation Rii(τ)=e−ai∣τ∣*R**ii*​(*τ*)=*e*−*a**i*​∣*τ*∣, where ai*a**i*​ is a real positive constant. Due to distant placement of sensors, yi(t1)*y**i*​(*t*1​) is uncorrelated to yj(t2)*y**j*​(*t*2​) for all i≠j*i*=*j* and for all t1*t*1​ and t2*t*2​. Mr. Eng found the ambient temperature differential of the School by taking the weighted average z(t)=∑i=1nbiyi(t)*z*(*t*)=∑*i*=1*n*​*b**i*​*y**i*​(*t*), where bi*b**i*​ are real constants.

**(a)**
Mr. Eng experimentally estimated the mean of the ambient temperature differential z(t)*z*(*t*) by observing its value for a long time and averaging these values. Unfortunately, Mr. Eng never took a course like EE7401, so he is not aware that such estimation makes sense only if z(t)*z*(*t*) is stationary and ergodic.

(i) Find ηz(t)*η**z*(*t*), the mean of z(t)*z*(*t*). Also find Rzz(t1,t2)*R**zz*(*t*1,*t*2), the autocorrelation of z(t)*z*(*t*). Is z(t)*z*(*t*) WSS?

(ii) Find Czz(τ)*C**zz*(*τ*), the autocovariance of z(t)*z*(*t*), and apply Slutsky’s theorem. Is z(t)*z*(*t*) mean-ergodic?

(iii) For the special case of ai=a*a**i*=*a* for all i*i*, z(t)*z*(*t*) becomes a special process. Which process is it?
[Hint: Check Rzz(τ)*R**zz*​(*τ*).]
*(13 Marks)*

**(b)**
To better engineer the temperature control, Mr. Eng Ine Er wants to predict the future temperature differential z(t+λ)*z*(*t*+*λ*) from the present value z(t)*z*(*t*), where λ>0*λ*>0. You can help Mr. Eng as follows:

(i) Find the optimal mean square predictor that predicts z(t+λ)*z*(*t*+*λ*) using z(t)*z*(*t*).

(ii) Find the least mean square (LMS) error P*P* for your predictor.
*(7 Marks)*

------

### 关键条件复述（中文）

**4(a)**

- 示威活动数 x(t)**x**(*t*) 是泊松过程，E[x(24)]=6⇒λ=6/24=0.25*E*[**x**(24)]=6⇒*λ*=6/24=0.25 次/小时
- (i) 求 x(24)**x**(24) 的方差
- (ii) 求 8 小时内示威 5 到 7 次的概率 P(5≤x(8)≤7)*P*(5≤**x**(8)≤7)
- (iii) 已知 6 小时内已发生 5 次 (x(6)=5)(**x**(6)=5)，求 8 小时内总次数 < 8 的条件概率 P(x(8)<8∣x(6)=5)*P*(**x**(8)<8∣**x**(6)=5)

**4(b)**

- 三状态：健康(H)、感染(I)、生病(S)
- 转移规则：
  - H → I: 概率 p*p*；H → S: 不可能
  - I → S: 概率 q*q*；I → H: 概率 p*p*
  - S → H: 概率 q*q*；S → S: 概率 1−q1−*q*；S → I: 不可能
- (i) 建立马尔可夫链，画图，求转移矩阵
- (ii) 求 p,q*p*,*q* 满足稳态概率 PH≥0.9*P**H*≥0.9 的条件

**5(a)**

- n*n* 个传感器，输出 yi(t)*y**i*(*t*) 为零均值 WSS，互不相关，自相关 Rii(τ)=e−ai∣τ∣*R**ii*(*τ*)=*e*−*a**i*∣*τ*∣
- 加权平均 z(t)=∑i=1nbiyi(t)*z*(*t*)=∑*i*=1*n**b**i**y**i*(*t*)
- (i) 求 z(t)*z*(*t*) 的均值 ηz(t)*η**z*(*t*) 和自相关 Rzz(t1,t2)*R**zz*(*t*1,*t*2)，判断是否 WSS
- (ii) 求自协方差 Czz(τ)*C**zz*(*τ*)，用 Slutsky 定理判断是否均值遍历
- (iii) 当所有 ai=a*a**i*=*a* 时，z(t)*z*(*t*) 是哪种特殊过程？

**5(b)**

- 用当前值 z(t)*z*(*t*) 预测未来值 z(t+λ)*z*(*t*+*λ*)（λ>0*λ*>0）
- (i) 求最优均方预测器
- (ii) 求最小均方误差 P*P*





### 

**4. (a)**  
_Stoopin’ Low:_ ____ Commissioner of Police Stoophen Lo is accused of stoopin’ low – using police brutality and violence – in his department’s fight against the youth ____. Mr. Lo starts each day with a peaceful mind, but too many ____ make him angry. Let **x(t)** = {number of ____ starting from time 0 to t, where t is measured in hours} be a Poisson process, such that the probability of k ____ is given by P{x(t) = k} = e^(-λt)(λt)^k / k!. It is known that, on average, there are 6 ____ per day, or E{x(24)} = 6.

(i) Find the variance of **x(24)**, the number of ____ in a day.

(ii) Mr. Lo spends hour 0 to hour 8 each day in his office, and remains peaceful as long as there are 4 or less ____. He gets agitated if there are 5 to 7 ____. Find the probability that Mr. Lo will be agitated in a day, that is, the probability that there are 5 to 7 ____ in 0 to 8 hours, or P{5 ≤ **x(8)** ≤ 7}.

(iii) If the number of ____ reaches 8 within his 8 hours in office, it makes Stoophen Lo getting angry and stoopin’ low. Today, it has been 6 hours in office, and so far, 5 ____ have taken place, or **x(6) = 5**. Find the conditional probability that Stoophen Lo will not be stoopin’ low today, that is, the conditional probability that there will be less than 8 ____ in 8 hours, or P{x(8) < 8 | **x(6) = 5**}.

[Hint: Express the conditional probability as the ratio of a joint probability and a marginal probability. Simplify the joint probability using the fact that non-overlapping Poisson intervals are independent.]

*(12 Marks)*

**(b)**  
_Seeing the Doctor:_ During an epidemic, Doctor See You Soon from the NTU Health Center classifies each NTU person as healthy, infected (but not sick), or sick.

- The probability that a healthy person becomes infected is \( p \), but a healthy person cannot become sick without getting infected first.
- An infected person may become sick with probability \( q \), or may become healthy with probability \( p \).
- Once a person is sick, he/she sees Doctor See You Soon. After seeing the Doctor, a sick person may become healthy with probability \( q \), while a sick person remains sick and needs to see Doctor See again with a probability \( 1 - q \). A sick person cannot become infected.

(i) Formulate the above problem as a Markov chain, where the states are healthy, infected, and sick. Draw the Markov chain and find the transition matrix.

(ii) Find the condition on \( p \) and \( q \) such that 90% or more of NTU people are healthy on an average, that is, the steady state probability \( P_{healthy} \geq 0.9 \).

*(8 Marks)*

**5.**  
*Engineering:* To verify the effectiveness of the new air-conditioning system in the School of EEE, Mr. Eng Ine Er placed \( n \) temperature sensors randomly in the School. Each sensor output is the difference between the measured temperature and the preset temperature. The \( i \)-th sensor output is a real zero mean wide-sense stationary (WSS) random process \( y_i(t) \) with autocorrelation \( R_{ii}(\tau) = e^{-a_i|\tau|} \), where \( a_i \) is a real positive constant. Due to distant placement of sensors, \( y_i(t_1) \) is uncorrelated to \( y_j(t_2) \) for all \( i \neq j \) and for all \( t_1 \) and \( t_2 \). Mr. Eng found the ambient temperature differential of the School by taking the weighted average \( z(t) = \sum_{i=1}^{n} b_i y_i(t) \), where \( b_i \) are real constants.

**(a)**  
Mr. Eng experimentally estimated the mean of the ambient temperature differential \( z(t) \) by observing its value for a long time and averaging these values. Unfortunately, Mr. Eng never took a course like EE7401, so he is not aware that such estimation makes sense only if \( z(t) \) is stationary and ergodic.

(i) Find \( \eta_z(t) \), the mean of \( z(t) \). Also find \( R_{zz}(t_1,t_2) \), the autocorrelation of \( z(t) \). Is \( z(t) \) WSS?

(ii) Find \( C_{zz}(\tau) \), the autocovariance of \( z(t) \), and apply Slutsky’s theorem. Is \( z(t) \) mean-ergodic?

(iii) For the special case of \( a_i = a \) for all \( i \), \( z(t) \) becomes a special process. Which process is it? [Hint: Check \( R_{zz}(\tau) \).]

*(13 Marks)*

**(b)**  
To better engineer the temperature control, Mr. Eng Ine Er wants to predict the future temperature differential \( z(t + \lambda) \) from the present value \( z(t) \), where \( \lambda > 0 \). You can help Mr. Eng as follows:

(i) Find the optimal mean square predictor that predicts \( z(t + \lambda) \) using \( z(t) \).

(ii) Find the least mean square (LMS) error \( P \) for your predictor.

*(7 Marks)*

---

### 关键条件复述（中文）

**4(a)**  
- 事件发生次数 \(x(t)\) 是泊松过程，\(E[x(24)] = 6 \Rightarrow \lambda = 0.25\)/小时  
- (i) 求 \(x(24)\) 的方差  
- (ii) 求 8 小时内发生 5–7 次事件的概率 \(P(5 \leq x(8) \leq 7)\)  
- (iii) 已知前 6 小时发生 5 次，求 8 小时内总次数 < 8 的条件概率 \(P(x(8) < 8 \mid x(6) = 5)\)

**4(b)**  
- 三状态：健康(H)、感染(I)、生病(S)  
- 转移规则：  
  - H → I: \(p\)；H → S: 不可能  
  - I → S: \(q\)；I → H: \(p\)  
  - S → H: \(q\)；S → S: \(1-q\)；S → I: 不可能  
- (i) 建立马尔可夫链，画图，求转移矩阵  
- (ii) 求 \(p, q\) 满足稳态概率 \(P_H \geq 0.9\) 的条件

**5(a)**  
- \(n\) 个传感器，输出 \(y_i(t)\) 为零均值 WSS，自相关 \(R_{ii}(\tau) = e^{-a_i|\tau|}\)，互相独立  
- 加权平均 \(z(t) = \sum_{i=1}^n b_i y_i(t)\)  
- (i) 求 \(z(t)\) 的均值 \(\eta_z(t)\) 和自相关 \(R_{zz}(t_1,t_2)\)，判断是否 WSS  
- (ii) 求自协方差 \(C_{zz}(\tau)\)，用 Slutsky 定理判断是否均值遍历  
- (iii) 当所有 \(a_i = a\) 时，\(z(t)\) 是何种特殊过程？

**5(b)**  
- 用当前值 \(z(t)\) 预测未来值 \(z(t+\lambda)\)，\(\lambda > 0\)  
- (i) 求最优均方预测器  
- (ii) 求最小均方误差 \(P\)





**2019**





### 

**1.**  
A binary random signal \( X \sim \text{Bern}(p), \, 0 \leq p \leq 1 \) is inputted to a random system. The system output is given by \( Y = 6X + 2Z \), where \( Z \) is a random variable independent to \( X \) and has a pdf  
\[
f_z(z) = \frac{1}{\sqrt{2\pi}} e^{-z^2/2}.
\]  

**(a)** Derive the conditional pdf \( f_{Y|X}(y \, | \, x) \).  
*(10 Marks)*  

**(b)** Estimate the value of the input \( X \) based on the system output \( Y \) that minimizes the probability of the wrong estimation.  
*(10 Marks)*  

**2.**  
A random variable has uniform pdf, \( X \sim U[0, 3] \). Given \( X = x \), a random variable \( Y \) has a pdf  
\[
f_{Y|X}(y \, | \, x) = 
\begin{cases} 
cxe^{-xy} & y \geq 0 \\ 
0 & \text{otherwise},
\end{cases}
\]  
where \( c \) is a constant.

**(a)** Find the marginal pdf \( f_Y(y) \).  
*(10 Marks)*

**(b)** Given \( Y = 1/3 \), estimate the value of X so that the mean square error of the estimation is minimized.  
*(10 Marks)*

**3. (a)**  
You have S$3 in your pocket consisting of 1 coin of 1 dollar, 2 coins of 50 cents, 3 coins of 20 cents and 4 coins of 10 cents. Two coins are randomly picked out from your pocket and 8 coins remaining in your pocket. Suppose that every coin has the same chance to be picked out.

(i) Compute the probability that you picked out 40 cents.  
*(5 Marks)*

(ii) Compute the probability that you picked out two coins of the same value.  
*(5 Marks)*

**(b)**  
In a fair coin experiment, define the process \( x(t) \) as \( x(t) = g(t) \) if the head shows, and \( x(t) = -g(t) \) if the tail shows, where \( g(t) \) is some given function of \( t \).

(i) What is \( \eta_x(t) = E\{x(t)\} \), the mean of \( x(t) \)?  

(ii) Is the process \( x(t) \) WSS (wide-sense stationary)?  
*(5 Marks)*

**(c)**  
Consider a complex random PPS (polynomial phase signal) process \( s(t) = \alpha \cdot \exp\left(j\left(\mathbf{p}_0 + \mathbf{p}_1 t + \mathbf{p}_2 t^2\right)\right) \), where \( \mathbf{p}_0, \mathbf{p}_1, \mathbf{p}_2 \) are independent non-zero mean real random variables, and \( \alpha \) is a real constant. If it is known that \( s(t) \) is WSS, show that \( \mathbf{p}_2 = 0 \).  
[Hint: Find the condition such that \( R_{ss}(t_1, t_2) = R_{ss}(\tau) \).]  
*(5 Marks)*

---

### 关键条件复述（中文）

**1**  
- 输入 \(X \sim \text{Bern}(p)\)  
- 系统输出 \(Y = 6X + 2Z\)，其中 \(Z \sim \mathcal{N}(0,1)\) 且与 \(X\) 独立  
- (a) 求条件 pdf \(f_{Y|X}(y|x)\)  
- (b) 基于输出 \(Y\)，以最小错误概率估计输入 \(X\)

**2**  
- \(X \sim U[0,3]\)  
- 条件 pdf：\(f_{Y|X}(y|x) = c x e^{-xy} \ (y \geq 0)\)，\(c\) 为常数  
- (a) 求边缘 pdf \(f_Y(y)\)  
- (b) 给定 \(Y=1/3\)，求最小 MSE 的 \(X\) 估计

**3(a)**  
- 口袋硬币：1枚1元，2枚50分，3枚20分，4枚10分（总值3元）  
- 随机取出2枚，每枚等可能被取  
- (i) 求取出总值为40分的概率  
- (ii) 求取出两枚相同面值的概率

**3(b)**  
- 公平抛硬币，若正面则 \(x(t)=g(t)\)，若反面则 \(x(t)=-g(t)\)  
- (i) 求均值 \(E[x(t)]\)  
- (ii) 判断 \(x(t)\) 是否 WSS

**3(c)**  
- 复随机多项式相位信号：\(s(t) = \alpha e^{j(p_0 + p_1 t + p_2 t^2)}\)  
- \(p_0, p_1, p_2\) 独立、非零均值实随机变量，\(\alpha\) 实常数  
- 已知 \(s(t)\) 是 WSS，证明 \(p_2=0\)  
- 提示：找 \(R_{ss}(t_1,t_2)=R_{ss}(\tau)\) 的条件





### 

**4. (a)**  
_McDonald’s:_ President Mcdonald Trump gets his food from McDonald’s every day. He orders different items each day and gets 50% discount on the total price (after all, he is the president). He further pays a tip equal to 50% of his previous day’s expenses. Let the total price of president Trump’s order on \( n \)-th day be modeled by a discrete-time real stationary white noise process \( v[n] \) with autocorrelation \( R_{vv}[m] = 3\delta[m] \). Let the president’s expenses at McDonald’s on \( n \)-th day be another process \( y[n] \). Since the president pays 0.5\( v[n] \) after discount, and pays a tip of 0.5\( y[n-1] \), his expenses on \( n \)-th day is \( y[n] = 0.5v[n] + 0.5y[n-1] \). Therefore, \( y[n] \) is the output of a linear system with transfer function
\[
H(z) = \frac{1}{2 - z^{-1}} \text{ when } v[n] \text{ is the input. In the following, help president Mcdonald Trump to find out the autocorrelation of } y[n].
\]

(i) Find \( S_{vv}(\omega) \), the power spectrum of the price.

(ii) Find \( S_{yy}(\omega) \), the power spectrum of the expenses.

(iii) Find \( R_{yy}[m] \), the autocorrelation of the expenses. You may use either one of the following hints.  
[Hint: frequency domain: Express \( S_{yy}(\omega) \) as a sum of two parts of the form
\[
\frac{\alpha}{1 - ce^{-j\omega}} + \frac{\beta e^{j\omega}}{1 - ce^{j\omega}} \text{ for appropriate constants } \alpha, \beta.
\]
Inverse Fourier transform of the first part is \( \alpha c^n u[n] \), while inverse Fourier transform of the second part is \( \beta c^{-n-1} u[-n-1] \). Now add both parts.]  
[Hint: time domain: Rewrite \( y[n] = 0.5v[n] + 0.5y[n-1] \) as \( y[n] \) equals to the sum of only present and past inputs (no past output terms like \( y[n-k] \) should remain). Using this expression, find \( E\{y[n]y[n+m]\} \) for \( m \geq 0 \). The \( m < 0 \) case may be found from symmetry.]

**(b)**  
_Modulation:_ Let \( w(t) = a(t) + jb(t) \) be a complex modulating process, where \( a(t) \) and \( b(t) \) are real jointly WSS processes with auto/cross correlations \( R_{aa}(\tau), R_{bb}(\tau), R_{ab}(\tau) \) and \( R_{ba}(\tau) \). Let \( x(t) = a(t) \cos(\omega_0 t) - b(t) \sin(\omega_0 t) \) be the real part of the modulated process.

(i) Find \( R_{ww}(t + \tau, t) \), the autocorrelation of \( w(t) \). Is \( w(t) \) WSS?

(ii) Find \( R_{xx}(t + \tau, t) \), the autocorrelation of \( x(t) \), and hence find the condition(s) on \( R_{aa}(\tau), R_{bb}(\tau), R_{ab}(\tau) \) and \( R_{ba}(\tau) \) such that \( x(t) \) is WSS.

**5. (a)**  
_Dementia:_ Prof. Dame N. Seah is suffering from dementia and keeps forgetting to bring her spectacle from her home to her office, or to bring it back from her office to her home. In the morning, Prof. Seah is fresh; if the spectacle is at her home, she remembers to take it to the office with a probability of 0.8. In the evening, Prof. Seah is tired; if the spectacle is at the office, she remembers to take it back home with a probability of only 0.4.

(i) Formulate the above problem as a Markov chain, where the states represent the spectacle is at the home or at the office. Draw the Markov chain and find the transition matrix.

(ii) Find the steady state probability \( p_{office} \) that the spectacle is at the office.

(iii) Will \( p_{office} \) (the steady state probability that the spectacle is at the office) increase if the probability 0.4 (as above, probability to take the spectacle back home from office) is increased?

*(11 Marks)*

**(b)**  
_Chilling Winter:_ Moving to Beijing, Qi Ling finds the winter to be very chilling. The temperature moves around zero degrees. Qi Ling modelled the temperature as a real WSS order 1 Markov process \( s(t) \) where \( t \) is measured in hour, and found that its autocorrelation is \( R_{ss}(\tau) = 5e^{-|\tau|/2} \). To better prepare against the chilling winter, Qi Ling wants to predict the temperature after 2 hours \( s(t+2) \) from the current temperature \( s(t) \).

(i) Determine the optimal predictor in the LMS (least mean square) error sense, that predicts \( s(t+2) \) using \( s(t) \).

(ii) Find the LMS error \( P \) for your predictor.

(iii) Qi Ling is not happy with the LMS error \( P \), and wants to reduce it further. So Qi Ling designs another predictor that predicts \( s(t+2) \) from both the current temperature \( s(t) \) and the temperature an hour ago \( s(t-1) \). Comment on how much \( P \) may be reduced using this second predictor.

*(9 Marks)*

---

### 关键条件复述（中文）

**4(a)**  
- 每日原价 \(v[n]\) 是实平稳离散白噪声，\(R_{vv}[m] = 3\delta[m]\)  
- 实际花费 \(y[n] = 0.5v[n] + 0.5y[n-1]\)，系统函数 \(H(z) = 1/(2 - z^{-1})\)  
- 求：  
  - (i) \(S_{vv}(\omega)\)  
  - (ii) \(S_{yy}(\omega)\)  
  - (iii) \(R_{yy}[m]\)

**4(b)**  
- 复调制过程 \(w(t) = a(t) + j b(t)\)，\(a(t), b(t)\) 实联合 WSS  
- 已调信号实部 \(x(t) = a(t)\cos(\omega_0 t) - b(t)\sin(\omega_0 t)\)  
- 求：  
  - (i) \(R_{ww}(t+\tau, t)\)，判断 \(w(t)\) 是否 WSS  
  - (ii) \(R_{xx}(t+\tau, t)\)，求 \(x(t)\) 为 WSS 时 \(R_{aa}, R_{bb}, R_{ab}, R_{ba}\) 满足的条件

**5(a)**  
- 教授记性差，眼镜在“家(H)”或“办公室(O)”  
- 早晨若在家，以 0.8 概率带到办公室  
- 晚上若在办公室，以 0.4 概率带回家  
- (i) 建立两状态马尔可夫链，画图，求转移矩阵  
- (ii) 求稳态概率 \(p_{office}\)  
- (iii) 若晚上带回家概率从 0.4 增加，\(p_{office}\) 是否增加？

**5(b)**  
- 温度过程 \(s(t)\) 实 WSS 一阶马尔可夫，自相关 \(R_{ss}(\tau) = 5e^{-|\tau|/2}\)  
- 用当前温度 \(s(t)\) 预测 2 小时后 \(s(t+2)\)  
- (i) 求最优 LMS 预测器  
- (ii) 求 LMS 误差 \(P\)  
- (iii) 若用 \(s(t)\) 和 \(s(t-1)\) 一起预测，评论 \(P\) 能减少多少







