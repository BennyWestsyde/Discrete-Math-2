***
## Proof Techniques
***

### Structural Induction

#### Summary:
Structural induction is a proof technique used to prove properties for recursively defined structures like strings, trees, or graphs.

#### Definitions:

- **Basis**
: The initial elements in the recursive definition that have property P.
- **Induction**
: The step where we assume the old items used to build a new item have property P and show that the new item also has property P.

#### Example:

Prove that the sum of the first n odd numbers is $n^2$.

Basis: $n = 1, 1$ is the first odd number and $1^2 = 1$.

Induction: Assume the sum of the first $k$ odd numbers is $k^2$. Now, consider $k+1$.

Sum of the first $k+1$ odd numbers $= k^2 + (2k + 1) = (k+1)^2$

#### Tricky Things to Remember:

- Structural induction is different from mathematical induction.
- Always make sure you have a valid basis step and an induction step.

something new
