Lemma 2.1.11
a) 
Let $x\in A^{o}$ be arbitrary. Let $\varepsilon > 0$ such that $B_{\varepsilon}(x) \subseteq A$. Then, $x\in B_{\varepsilon}(x) \subseteq A$. 

b)

___Definition 2.8.1___
Let $A \subseteq \mathbb{R}^n$  and $f$ a real-valued function defined on $A$. 
- A point $p$ is a __(global) maximum of__ $f$ __on__ $A$ if $\forall x \in A.(f(p) \ge f(x))$.
	If so, $p$ is the __(global) maximum value of__ $f$ __on__ $A$.
- If a maximum value of $f$ on $A$ exists, then $f$ __attains a (global) maximum on__ $A$.
Similar definition for minimum.

___Theorem 2.8.8 (Least Upper Bound Principle/Completeness of $\mathbb{R}$)___
Let $S \subseteq \mathbb{R}$. If $S$ has an upper bound, then the supremum of $S$ exists.

___Corollary 2.8x.1___
Let $S \subseteq \mathbb{R}$. If $S$ has a lower bound, then the infimum of $S$ exists.

Proof: 
Consider the set $P = \{-x : x \in S\}$. Note that $P$ has an upper bound and hence has a supremum. We have $\inf(S) = -\sup(P)$. 

___Theorem 2.8.7 (Extreme Value Theorem)___
If $A \subseteq \mathbb{R}^n$ is a non-empty compact set and the map $f : A \to \mathbb{R}$ is continuous, then $f$ attains maximum and minimum values at points of $A$.

Proof:
It suffice to show that $f$ attains a maximum on $A$ as the proof for minimum is similar.
Let $A \subseteq \mathbb{R}^n$ be an arbitrary non-empty compact set. By __Theorem 2.6.35__ , $f(A)$ is compact (done by __Lemma 2.8x.2__) and thus closed and bounded by __Bolzano-Weierstrass Theorem__. By __Theorem 2.8.8__, there exists $M  = \sup\{y : y \in f(A)\}$.
Let $\varepsilon > 0$ be arbitrary. 
By definition, there exists $z \in f(A)$ such that $M - \varepsilon < z \le M$. If $z = M$ then $M \in f(A)$.  Consider $z \ne M$, then $z \in B_{\varepsilon}(M) \cap f(A) \ne \varnothing$.
Thus, $M$ is a limit point of $f(A)$. Since $f(A)$ is closed, $M \in f(A)$. 

___Lemma 2.8x.2___
- If $S \subseteq \mathbb{R}$ closed and bounded above, then $S$ has a maximum element.
- If $S \subseteq \mathbb{R}$ closed and bounded below, then $S$ has a minimum element.
In particular, if $S \subseteq \mathbb{R}$  is compact, then $S$ has a maximum and minimum element.

Proof:
_Case 1: $S$ is bounded above, thus it has a supremum $M$ by __Theorem 2.8.8__._
Let $\varepsilon > 0$ be arbitrary. 
By definition, there exists $z \in S$ such that $M - \varepsilon < z \le M$. If $z = M$ then $M \in S$.  Consider $z \ne M$, then $z \in B_{\varepsilon}(M) \cap S \backslash \{M\} \ne \varnothing$.
Thus, $M$ is a limit point of $S$. Since $S$ is closed, $M \in S$. 

_Case 2: $S$ is bounded below, thus it has an infimum $m$ by __Corollary 2.8x.1__. _
Let $\varepsilon > 0$ be arbitrary.
By definition, there exists $z \in S$ such that $m \le z < m + \varepsilon$. If $z = m$ then $m \in S$.  Consider $z \ne m$, then $z \in B_{\varepsilon}(m) \cap S \backslash \{m\} \ne \varnothing$.
Thus, $m$ is a limit point of $S$. Since $S$ is closed, $m \in S$. 

___Lemma 2.8.14___
Let $A \subseteq \mathbb{R}^n$ be closed and unbounded. Let $f$ be a continuous real-valued function on $A$. If $f(x) \to -\infty$ as $\| x \|  \to \infty$, then $f$ attains a maximum on $A$.

Proof:
Assume $f(x) \to -\infty$ as $\| x \| \to \infty$. 
	_Claim: $f(A)$ is bounded above._
	Proof:
	Assume for contradiction that $f$ is unbounded above, then there exists a sequence  $\{x(k)\}_k$  in $A$ such that $\displaystyle \lim_{k \to \infty} {f(x(k))} = \infty$.  Note that $\| x\| \ge 0$ for all $x \in A$, consider two cases
	_Case 1:  $\{\|x(k)\|\}_k$ is unbounded._
	By assumption, $f(x(k)) \to -\infty$ as $k \to \infty$. A contradiction.
	_Case 2:  $\{\|x(k)\|\}_k$ is bounded above._
	By __Theorem 2.8.8__, there exists $\displaystyle M = \sup_{k \in \mathbb{N}^{+}}\{x(k)\}$. By definition, there exists a subsequence $\{x(m(k))\}_k$ that converges to $M$. Since $f$ is continuous at $A$, by __Theorem 2.6.5__, $\infty = \displaystyle \lim_{k \to \infty} f(x(k)) = \lim_{x \to  M} f(x) = f(M)$. Contradiction.
	Hence, the claim.
	
Since $f(A)$ is bounded above, by __Theorem 2.8.8__, there exists $M = \sup\{f(A)\}$. By definition, there is a sequence $\{y(k)\}_k$ in $A$ such that $f(y(k)) \to M$ as $k \to \infty$. 
	_Claim: $\{y(k)\}_k$ is bounded._
	Proof:
	Assume $\{y(k)\}_k$ is unbounded, by assumption $f(y(k)) \to -\infty$ as $k \to \infty$, contradiction.

From the claim, it we can deduce that $\{\| y(k) \|\}_k$ is bounded above, say by $S$. Consider the closed ball $\overline{B_{S}(0)}$, notice that $\{y(k)\}_k$ is contained in $\overline{B_{S}(0)}$ since $\forall k \in \mathbb{N}^+.(\| y(k)\| \le S)$. Since $\overline{B_{S}(0)}$ is compact, by __Bolzano-Weierstrass Theorem__, $f(\overline{B_S(0)})$ is closed. Because $\{f(y(k))\}_k$ converges to $M$, $M \in f(\overline{B_S(0)}) \subseteq f(A)$. Hence $f$ attains a maximum in $A$. 

