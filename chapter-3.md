Definition 3.1.1.
Let $A\subseteq \mathbb{R}$ and $f : A \to \mathbb{R}^m$. Let $a \in A^o$. **The derivative of $f$ at $a$** is defined to be  $$f'(a)  =\lim_{h\to 0} \frac{f(a+h) - f(a)}{h}$$
provided the limit exists. If the limit exists, then $f$ is **differentiable at** $a$.

We can show $$f'(a) = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}$$
Proof:
	(TBC)

Note definition 3.1.1. only defines derivatives on interior points.

Lemma 3.1.3.
Let $A\subseteq \mathbb{R}^m$, $f = (f_1, \ldots, f_m) : A \to \mathbb{R}^m$, and $a\in A^o$. $f$ is **differentiable at** $a$ if and only if $f_i$ is differentiable at $a$ for all $i \in \mathbb{N}$, $1\le i \le m$. If so, $$f'(a) = (f_1'(a), \ldots, f_m'(a)) = \begin{bmatrix}f_1'(a) \\ \vdots \\ f_m'(a) \end{bmatrix}$$
Proof:
	(TBC)

Theorem 3.1.6.
Let $A\subseteq\mathbb{R}$, and let $f, g$ be $\mathbb{R}^m-$valued function defined on $A$.  Let $a\in A^o$, $\lambda\in\mathbb{R}$, and $\varphi : A \to \mathbb{R}$. Then, the following holds
- (Linearity) If $f,g$ is differentiable at $a$, $f + \lambda g$ is differentiable at $a$ and $$(f+\lambda g)'(a) = f'(a) + \lambda g'(a)$$
- (Scalar Product) If $f, \varphi$ is differentiable at $a$, then $\varphi f$ is differentiable at $a$ and $$(\varphi f)'(a) = \varphi'(a)f(a) + \varphi(a)f'(a)$$
- (Dot Product) If $f, g$ is differentiable at $a$, then $f \cdot g$ is differentiable at $a$ and $$(f\cdot g)'(a) = f'(a)\cdot g(a) + f(a)\cdot g'(a)$$
Proof:
	(TBC)

Lemma 3.1.7. (Chain Rule)
Let $A, B \subseteq \mathbb{R}$. Let $\varphi : A \to B$ and $f : B \to \mathbb{R}$. Let $a \in A^o$ such that $\varphi(a) \in B^o$. If $\varphi$ is differentiable at $a$ and $f$ is differentiable at $\varphi(a)$, then $$(f \circ \varphi)'(a) = f'(\varphi(a))\varphi'(a)$$
Proof:
	(TBC)

Theorem 3.1.9.
Let $A\subseteq \mathbb{R}$ and $f : A \to \mathbb{R}^m$. Let $a \in A^o$. $f$ is differentiable at $a$ if and only if there is a linear map $L : \mathbb{R} \to \mathbb{R}^m$ such that $$\lim_{h\to 0} \frac{f(a+h) - f(a) - L(h)}{h} = 0$$
at which $L(h) = f'(a) h$. 

Proof:
	(TBC)

Definition 3.1.10.
Let $A\subseteq \mathbb{R}$, $f: A \to \mathbb{R}^m$ , $a \in A^o$. If $f$ is differentiable at $a$, then the linear map $df_a : \mathbb{R} \to \mathbb{R}^m$ defined by $df_a(h) = f'(a) h$ is **the differential of $f$ at $a$.**

Definition 3.2.2 
Let $A \subseteq \mathbb{R}^n$ and let $f: A \rightarrow \mathbb{R}^m$. Let $a$ be an interior point of $A$. Fix $1 \leq j \leq n$. Let $\left\{e_1, \ldots, e_n\right\}$ be the standard basis for $\mathbb{R}^n$. The $j$ th partial derivative of $f$ at $a$ is given by
$$
\partial_j f(a):=\lim _{h \rightarrow 0} \frac{f\left(a+h e_j\right)-f(a)}{h}
$$
provided the limit exists. The $j$ th partial derivative of $f$ is the function $\partial_j f: U \rightarrow \mathbb{R}^m$, where $U$ is the set of points $a \in A$ such that $\partial_j f(a)$ exists.

Lemma 3.2.7 
Let $A \subseteq \mathbb{R}^n$ and let $f=\left(f_1, \ldots, f_m\right): A \rightarrow \mathbb{R}^m$. Let $a$ be an interior point of $A$. The $j$ th partial of $f$ at $a$ exists if and only if for every $i \in\{1, \ldots, m\}$, the $j$ th partial of the component function $f_i: A \rightarrow \mathbb{R}$ at $a$ exists. If so,
$$
\partial_j f(a)=\left(\partial_j f_1(a), \ldots, \partial_j f_m(a)\right) .
$$
Definition 3.3.1 
Let $A \subseteq \mathbb{R}^n$ and let $f: A \rightarrow \mathbb{R}^m$ be a function. Let $a$ be an interior point of $A$. Fix a vector ${ }^3 v \in \mathbb{R}^n$. The directional derivative of $f$ at $a$ in the direction $v$ is given by
$$
D_v f(a)=\lim _{h \rightarrow 0} \frac{f(a+h v)-f(a)}{h}
$$
The directional derivative of $f$ in the direction $v$ is the function $D_v f: U \rightarrow \mathbb{R}^m$, where $U$ is the set of points $a \in A$ such that $D_v f(a)$ exists.

Lemma 3.3.5 
Let $A \subseteq \mathbb{R}^n$ and let $f=\left(f_1, \ldots, f_m\right): A \rightarrow \mathbb{R}^m$. Let $a$ be an interior point of $A$. Fix $v \in \mathbb{R}^n$. Then $D_v f(a)$ exists if and only if $D_v f_i(a)$ exists for every $i \in\{1, \ldots, m\}$. If so,
$$
D_v f(a)=\left(D_v f_1(a), \ldots, D_v f_m(a)\right) .
$$
Theorem 3.3.10 Let $A \subseteq \mathbb{R}^n$ and let $f: A \rightarrow \mathbb{R}^m$ be a function. Let $a$ be an interior point of $A$. If $f$ is differentiable at $a$, then for all $v=\left(v_1, \ldots, v_n\right) \in \mathbb{R}^n$,
$$
D_v f(a)=\sum_{j=1}^n v_j \partial_j f(a)
$$

Theorem 3.2.8 
Let $A \subseteq \mathbb{R}^n$. Let $f: A \rightarrow \mathbb{R}^m$ and $g: A \rightarrow \mathbb{R}^m$. Let $a$ be an interior point of $A$. Fix $1 \leq j \leq n$. Let $\lambda \in \mathbb{R}$ and let $\varphi$ be a real-valued function defined on $A$.
(a) (Linearity) If $\partial_j f(a)$ and $\partial_j g(a)$ both exist, then $\partial_j(f+\lambda g)(a)$ exists and
$$
\partial_j(f+\lambda g)(a)=\partial_j f(a)+\lambda \partial_j g(a) .
$$
(b) (Scalar product) If $\partial_j f(a)$ and $\partial_j \varphi(a)$ both exist, then $\partial_j(\varphi f)(a)$ exists and
$$
\partial_j(\varphi f)(a)=f(a) \partial_j \varphi(a)+\varphi(a) \partial_j f(a) .
$$
(c) (Dot product) If $\partial_j f(a)$ and $\partial_j g(a)$ both exist, then $\partial_j(f \cdot g)(a)$ exists and
$$
\partial_j(f \cdot g)(a)=\partial_j f(a) \cdot g(a)+f(a) \cdot \partial_j g(a) .
$$

Definition 3.4.1
Let $A \subseteq \mathbb{R}^n$, $f: A \to \mathbb{R}$, $a\in A^o$. The __gradient of__ $f$ __at__ $a$ is denoted $\nabla f(a)$ and given by the $n$-dimensional vector $$\nabla f(a) = (\partial_1 f(a), \ldots, \partial_n f(a))$$
provided the partial derivatives $\partial_1 f(a), \ldots, \partial_n f(a)$ all exists.

Theorem 3.4.3 
Let $A \subseteq \mathbb{R}^n$ and let $f: A \rightarrow \mathbb{R}$ be a real-valued function. Let $a$ be an interior point of $A$. If $f$ is differentiable at $a$, then for all $v=\left(v_1, \ldots, v_n\right) \in \mathbb{R}^n, D_v f(a)$ exists and
$$
D_v f(a)=\nabla f(a) \cdot v=(\nabla f(a))^T v .
$$

Definition 3.4.6
Let $U \subseteq \mathbb{R}^n$ be open and let $f: U \rightarrow \mathbb{R}$ be a real-valued function. Assume all partial derivatives of $f$ exist on all of $U$. The gradient of $f$ (or gradient vector field of $f$ ) is the function $\nabla f: U \rightarrow \mathbb{R}^n$ given by $\nabla f(a)=\left(\partial_1 f(a), \ldots, \partial_n f(a)\right)$ for all $a \in U$.

Lemma 3.4.9
Let $A \subseteq \mathbb{R}^n$ and let $f: A \rightarrow \mathbb{R}$ be a real-valued function. Let $a$ be an interior point of $A$. Assume $f$ is differentiable at $a$ and $\nabla f(a) \neq 0$. Both of the following hold:
(a) The maximum of $D_u f(a)$ over all unit vectors $u$ occurs when $u=+\frac{\nabla f(a)}{\|\nabla f(a)\|}$ and the maximum value is $\|\nabla f(a)\|$.
(b) The minimum of $D_u f(a)$ over all unit vectors $u$ occurs when $u=-\frac{\nabla f(a)}{\|\nabla f(a)\|}$ and the minimum value is $-\|\nabla f(a)\|$.

This lemma formalizes two notions.
	First, the gradient $\nabla f(a)$ points in the direction of steepest ascent at $a$.
	Second, the norm $\|\nabla f(a)\|$ is the rate of change of $f$ in this direction.

_Every tangent vector v at a point p of a set S written in implicit form is orthogonal to
$\nabla f(p)$. Moreover, the gradient $\nabla f(p)$ is orthogonal to the tangent plane of $S$ at $p$._