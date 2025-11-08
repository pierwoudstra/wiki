[[mathematics]]

Proof by contrapositive

P -> Q is equivalent to ~Q -> ~P

Assume Q is false, then P is false because $\square$

Thm: $\forall n \in Z . iseven(n^2) \rightarrow iseven(n)$
Pf. Suppose $n \in Z$. Proof by contrapositive. Assume $n$ is odd, then 
$$n = 2k + 1$$, where $k\in Z$.
If
$$n = 2k+1$$
then
$$n^2 = (2k+1)^2 $$
$$= 4k^2+4k+1 $$
$$= 2(2k^2 + 2k) + 1 = 2m + 1$$
Therefore $n^2$ is odd. 
Using the contrapositive, this means that if $n^2$ is even, $n$ is also even. $\square$