[[mathematics]]

# *Relations*
A relation can be described by a set of ordered pairs. Here the first item of the ordered pair is has a certain relation to the second item.

Examples of relations are: $=, \subset, >$, etc.

A relation $R$ between two sets $A$ and $B$ is a subset of the Cartesian product of $A$ and $B$:
$R \subseteq A \times B$.

For example if we have set $A = \{1, 2, 3\}$ and relation $R$ is the equals relation ($=$), then we have $R = \{(1, 1), (2, 2), (3,3)\}$.
This set $R$ is a subset of $A \times A$.

*Properties of relations*
---
A relation is said to be **reflexive** if $(a,a) \in R$ for every $a \in A$, where $A$ is the set on which $R$ operates. 

Take the set $A = \{1, 2, 3\}$ for example. The relation $R$ on the set $A$ is reflexive if $(1,1)$, $(2,2)$ and $(3,3)$ are elements of $R$.

A relation $R$ on set $A$ is **symmetric** if, whenever $aRb$ then also $bRa$.
For example, the parallel relation between lines $||$ is symmetric because whenever a line $a$ is parallel to line $b$, then line $b$ is parallel to line $a$.

The relation can be symmetric or not, but also **antisymmetric**. 

A relation is antisymmetric if no two distinct elements are symmetrically related.
This means two elements can only relate in both directions if they are in fact the same element. 
This is the case whenever $aRb \land bRa \implies a=b$. This means that $R$ is symmetric only when $a$ and $b$ are the same value. Thus $R$ is not antisymmetric whenever there are values $a$ and $b$, which are not equal, and $aRb \land bRa$ is true.

*Transitive relations*
---
*Operations on relations*
---
$R \circ S = \{(a,c)|(a,b) \in R \land (b,c) \in S\}$
$R^2 = R \circ R$
$R^n \subseteq R \times R$

*Closures of relations*
---
$reflexive(R) = R \cup\{(a,a)|a\in A\}$
$symmetric(R) = R\cup\{(b,a)|(a,b)\in R\}$
$transitive(R) = R \cup \{(a,c)|(a,b) \in R \land (b,c) \in R )\}$


*Equivalence relation*
---
 A relation which is reflexive, symmetric and transitive is called an **equivalence relation**. 

*Equivalence classes*
---
$[x] = \{y|(x,y) \in R\}$
For example, if $R$ is an equivalence relation like $\{(1,1), (1,2), (2,1), (2,2), (3,3)\}$ then equivalence class $[1]=\{1, 2\}$ while the equivalence class $[3]=\{3\}$.

*Partial ordering relation*
---
**Partial ordering relations** are almost the same as equivalence relations except that they are *antisymmetric* and not symmetric. Examples of there relations are $\subseteq,\le$ and $|$ (divides). 





