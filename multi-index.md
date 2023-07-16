Let $x$ be a vector in $\mathbb{R}^n$. Let $\alpha$ be an integer vector, that is, a vector of $\mathbb{N}_0^n$. Define $x^\alpha = x_1^{\alpha_1}\cdot x_2^{\alpha_2}\cdots x_n^{\alpha_n}$. Define $\alpha! = \alpha_1!\cdot\alpha_2!\cdots\alpha_n!$.

Let $x_1,x_2,...,x_k\in \mathbb{R}^n$. Then 
$$(x_1+x_2+...+x_k)^\alpha = \sum _{(*)} \frac{\alpha!}{\beta_1!\beta_2!...\beta_k!} x_1^{\beta_1}x_2^{\beta_2}...x_k^{\beta_k}$$
where $(\beta_1,\beta_2,\cdots,\beta_k)$ is a partition of $\alpha$, that is, $\beta_1+...+\beta_k=\alpha$, and the summation condition $(*)$ is running through the set 
$$
\{ (\beta_i): \beta_1+...+\beta_k=\alpha \}
$$

To prove this, we first assume the formula is true for scalar $x_i,\alpha,\beta_i$. Now for vector $x_i,\alpha,\beta_i$, we want to prove
$$
(\sum x_i)^\alpha
=\sum_{(*)} \frac{\alpha!}{\Pi_i\beta_i!}\Pi_i x_i^{\beta_i}
$$

Let $I=\{1,\cdots,k\}$ and $J=\{1,\cdots,n \}$. Let $i\in I, j\in J$ be the running index. Then,

$\begin{aligned} 
(\sum x_i)^\alpha
&=  \Pi_j (\sum_i x_i)_j^{\alpha_j} 
\,\,\,\,\,\,\,\,\,\,\textrm{-- by multi-index defintion} \\
&=  \Pi_j (\sum_i x_{ij})^{\alpha_j} \\
& = \Pi_j \sum_{(**)} \frac{\alpha_j!}{\Pi_i \beta_{ij}!} \Pi_i x_{ij}^{\beta_{ij}} 
\,\,\,\,\,\,\,\,\,\,\textrm{-- by scalar formula}\\
&= \sum_{(***)}\frac{\Pi_j\alpha_j!}{\Pi_{ij}\beta_{ij}!} \Pi_{ij}x_{ij}^{\beta_{ij}} 
\,\,\,\,\,\,\,\,\,\,\textrm{-- switching product and summation}\\
&=\sum_{(***)} \frac{\alpha!}{\Pi_i\beta_i!}\Pi_i x_i^{\beta_i}
\,\,\,\,\,\,\,\,\,\,\textrm{-- by multi-index defintion}
\end{aligned}$


where the summation condition $(**)$ is for each $j$, the tuple $(\beta_{ij})$ runs through a patition of $\alpha_j$, the summation condition $(***)$ is taking a tuple $(\beta_{ij})$ from a partition of $\alpha_j$ for each $j$. Notice that it is exactly taking the vector partition of $\alpha$, that is $(***)=(*)$.
