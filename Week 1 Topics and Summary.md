# Maps#

## 1.1. Parametric Curves##
Parametric curves are maps from $\mathbb{R} \rightarrow \mathbb{R}^{n}$ , for example define $\gamma(t) = (\cos(t), \sin(t))$ for 
$t\in\mathbb{R}$, this maps a circle. Another notable map is
$$f(t) = (\cos(t), \sin(t), t)$$
which maps a __helix__.

A parametric curve $\gamma : I \rightarrow \mathbb{R}^n$ for some interval $I \in \mathbb{R}$ describes a motion with position $\gamma(t)$ and time $t$. 
The velocity is given by 
$$\gamma'(t) = \lim_{h\rightarrow 0} \frac{\gamma(t+h) - \gamma(t)}{h}$$

The map $\gamma$ can be represented as $\gamma(t) = (\gamma_1(t), \cdots, \gamma_n(t))$ where $\gamma_{i} : I \rightarrow \mathbb{R}^n$  for each $i \in \mathbb{N} \cap [1, n]$. Using fancy analysis or some simple calculations we can show that 
$$ \gamma'(t) = (\gamma_1(t), \cdots, \gamma_n(t))$$

The __speed__ of the object at time $t$ is the magnitude $\lVert \gamma'(t) \rVert$.
The __direction of motion__ is the unit tangent vector denoted $T = T(t) = \frac{\gamma'(t)}{\lVert \gamma'(t) \rVert}$.

Conversely, we can _integrate_ a motion as in single-variable calculus, we have (this is not rigorous at all, will explain in later notes)
$$\gamma(t) = \int_{0}^{t} \gamma'(s) ds = \Bigg(\int_{0}^{t} \gamma_1(s) ds, \cdots, \int_{0}^{t} \gamma_n(s) ds \Bigg)$$

#### Principal unit normal (_orthogonal_ to $T$): ####
$$ N(t) = \frac{T'(t)}{\lVert T'(t) \rVert} $$

Given that $T$ and $N$ are orthogonal, if we were to put another orthogonal vector $B$, notice that $B$ and $-B$ are both orthogonal to $T$ and $N$, we do the following to avoid confusion. 
We define the __binormal unit vector__ to be the unique vector such that $\{ T, N, B \}$ are positively-oriented. This ordered basis forms the __Frenet frame__ (Frenet-Serret Frame or TNB Frame).

To find $B$ algebraically, we can calculate the cross-product $B = T \times N$.

The __trace__ of $\gamma : I \rightarrow \mathbb{R}^n$ is the image of $\gamma$, $\gamma(I)$. 

		