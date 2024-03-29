[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

## Proof:
$f(n) = o(g(n))$ - This means that for any positive constant $c > 0$, there exists an $n<sub>0</sub>$ such that for all $n ≥ n<sub>0</sub>$, $f(n) < c * g(n)$. <br />
$f(n) = O(g(n))$ - This means that we have to find some constant $c' > 0$ and some $n<sub>0</sub>$' such that for all n ≥ n<sub>0</sub>', $f(n) ≤ c' * g(n)$.
`<` `>` `≤` and `≥`

Given f(n) = o(g(n)), by definition for all c > 0, there exists n<sub>0</sub> such that for all n ≥ n<sub>0</sub>, we have $f(n) < c * g(n)$.

Choosing any c > 0, say c = 1. Then there exists n<sub>0</sub> such that for all n ≥ n<sub>0</sub>, f(n) < g(n).

This directly gives us that f(n) ≤ g(n) for all n ≥ n<sub>0</sub> because < implies ≤ as well.

Therefore, we can set C = 1 and  the same n<sub>0</sub> from our little-o definition to satisfy the big-O definition

Hence, we have shown that if f(n) = o(g(n)), then f(n) = O(g(n)), with C = 1 and the  n<sub>0</sub> given by the definition of little-o.

