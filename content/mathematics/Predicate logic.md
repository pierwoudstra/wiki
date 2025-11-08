[[logic]]

# Predicate logic

> Is $r < 4$ a correct proposition?

We defined a proposition as something which can be either true or false, and while we can give truth values to $3 < 4$ and $7 < 4$ (true and false respectively), here we are faced with a variable $r$.
Statements with variables don't have truth values, they are called **predicates**.

Which of the following is a proposition and which a predicate?
- Roses are red.
- $2 + 2 = 5$
- $a$ is red.
- Some numbers are smaller than four.

This last one can be a bit tricky because it looks like the predicate in the beginning. The difference in this statement, which makes it a proposition and not a predicate is that we are using *some number* and not just the variable $r$, which could be anything.

Formally this is called a **quantifier**, and it is used to turn a predicate into a proposition by adding some information about the variable that we are using.

The quantifier we used in this example is called the **existential quantifier** and if formally denoted by: $\exists x$ which means *there is at least one x*.

To use this to make the proposition we had in the beginning we write:
$$\exists r(r<4)$$
This means there is at least one number $r$ which is smaller than four. This proposition evaluates to true, as there are infinitely many numbers smaller than four.

The other quantifier we have is called the **universal quantifier**, it looks like this:
$\forall x$ and is read *for all x*. This means that you are stating the proposition for all values of $x$, for example:
$$\forall x(x<4)$$This evaluates to false, as is it not true that all numbers are smaller than four.