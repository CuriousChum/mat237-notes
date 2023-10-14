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



