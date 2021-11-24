# mathjax 语法说明





如果有一系列的等式需要写，并且等号需要对齐，那么可以用 `\begin{align}…\end{align}`。
每次换行都要用 `\\`，新的一行需要在需要对齐的地方使用 `&`。



### 根式

$$
\begin{align}
\sqrt{37} & = \sqrt{ \frac{73^2-1}{12^2}} \\
& = \sqrt{ \frac{73^2}{12^2} \cdot \frac{73^2-1}{73^2}} \\ 
& = \sqrt{ \frac{73^2}{12^2}}\sqrt{ \frac{73^2-1}{73^2}} \\
& = \frac{73}{12} \sqrt{1 - \frac{1}{73^2}} \\ 
& \approx \frac{73}{12} \left(1 - \frac{1}{2 \cdot73^2} \right)
\end{align}
$$

### 上标下标


$$
% 这个是为了导入数学宏包，之后才能调用mathrsfs中的方法
\begin{align}
& (f,K^{'}_{x}y+K^{''}_{x}y)_{F}\\
&=(f^{'}+f^{''},K^{'}_{x}y+K^{''}_{x}y)_{F}\\
&=(f^{'},K^{'}_{x}y)_{F}+(f^{''},K^{''}_{x}y)_{F}+(f^{'},K^{''}_{x}y)_{F}+(f^{''},K^{'}_{x}y)_{F}\\
&=(f^{'},K^{'}_{x}y)_{F}+(f^{''},K^{''}_{x}y)_{F}\\
&=(f^{'}(x),y)_{Y}+(f^{''}(x),y)_{Y}\\
&=(f^{'}(x)+f^{''}(x),y)_{Y}\\
&=(f(x),y)_{Y}\\
&=(f,K_{x}y)_{F}
\end{align}
$$


### 方程组

$$
\begin{equation}   
\left\{
  \begin{array}{r1}
  a_{0}+a_{1}x_{0}+...+a_{n}x_{0}^{n}=y_{0} \\
  a_{0}+a_{1}x_{1}+...+a_{n}x_{1}^{n}=y_{1} \\
  \cdots\\
  a_{0}+a_{1}x_{n}+...+a_{n}x_{n}^{n}=y_{n} 
  \end{array}
\right.
\end{equation}
$$

$$
\left \{ 
\begin{array}{c}
a_1x+b_1y+c_1z=d_1 \\ 
a_2x+b_2y+c_2z=d_2 \\ 
a_3x+b_3y+c_3z=d_3
\end{array}
\right.
$$







