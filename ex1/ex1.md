# ex1

## 1.1

$$
\begin{gathered}
  \alpha = (0.4, 0.6)
\\
  \beta = (0.5, 0.5)
\end{gathered}
$$

transport plan:

$$
r = \begin{pmatrix}
    0.4 & 0.1
  \\
    0 & 0.5
\end{pmatrix}
$$

verify that constraints are met:

$$
\begin{gathered}
  \sum_i r_{ij} = \alpha_i \leq \alpha_i
\\
  \sum_j r_{ij} = \beta_j
\end{gathered}
$$

## 1.2

$$
\begin{gathered}
  c_l(x,y) = |x-y|
\\
  c_q(x,y) = \frac{1}{2} |x-y|^2
\end{gathered}
$$

## 1.3

consider a regular tetrahedron:

$$
\begin{gathered}
  p_1 = (-1,0,0)
\\
  p_2 = (1,0,0)
\\
  q_1 = (0,-1,1)
\\
  q_2 = (0,1,1)
\end{gathered}
$$

let the measures be combinations of delta functions centered in the vertices:

$$
\begin{gathered}
  \mu = \delta_{p_1} + \delta_{p_2}
\\
  \nu = \delta_{q_1} + \delta{q_2}
\end{gathered}
$$

we arrive to a discrete transportation problem, where the cost matrix is
proportional to a matrix of ones:

$$
\begin{gathered}
  c(p_1, q_1) = c(p_2, q_2) = c(p_1, q_2) = c(p_2, q_1) = \frac{3}{2}
\end{gathered}
$$

thus, any feasible transportation plan $r$ is optimal:

$$
r = \begin{pmatrix}
    \alpha & 1 - \alpha
  \\
    1 - \alpha & 1
\end{pmatrix}
\quad \forall \alpha \in [0,1]
$$

## 1.4

TODO: the result should be softmin, cf "ml in physics"
