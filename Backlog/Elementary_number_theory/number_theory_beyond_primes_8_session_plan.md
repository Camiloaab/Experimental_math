# Suggested 8-Session Plan: Elementary Number Theory Beyond Primes

## Module title

**Finite Arithmetic, Reciprocity, and Point Counting**

## Guiding theme

Arithmetic modulo \(n\) turns number theory into a finite experimental world. In these finite worlds we can draw tables, plot graphs, count solutions, iterate maps, and discover patterns that lead to reciprocity laws, finite geometry, and the first hints of the Weil conjectures.

---

## Overview of the 8-session arc

1. Modular arithmetic creates finite worlds.
2. Multiplication modulo \(p\) has cyclic structure.
3. Squares reveal hidden residue patterns.
4. Quadratic reciprocity shows a surprising symmetry.
5. Cubes reveal that the quadratic analogy breaks.
6. Eisenstein integers repair the symmetry.
7. Counting solutions turns arithmetic into geometry.
8. Elliptic curves and Weil show that geometry controls point counts.

In one sentence:

> This module begins with arithmetic tables and ends with the idea that deep geometry governs arithmetic over finite fields.

---

# Session 1 — Modular arithmetic as a finite universe

## Central question

What does arithmetic look like when numbers wrap around?

## Experiments

- Construct addition tables modulo \(n\).
- Construct multiplication tables modulo \(n\).
- Visualize tables as heatmaps.
- Compare prime moduli and composite moduli.
- Identify units and zero divisors.
- Plot maps \(x\mapsto ax\mod n\).

## Main discoveries

- Prime moduli behave like fields.
- Composite moduli have zero divisors.
- Modular arithmetic creates finite algebraic worlds.

## Mathematical shadows

- Rings \(\mathbb Z/n\mathbb Z\).
- Fields \(\mathbb F_p\).
- Units modulo \(n\).

---

# Session 2 — Powers, cycles, and primitive roots

## Central question

What happens when we repeatedly multiply by the same number modulo \(p\)?

## Experiments

- Compute powers \(a,a^2,a^3,\dots\mod p\).
- Find periods.
- Draw cycles of powers.
- Search for primitive roots modulo \(p\).
- Count primitive roots.
- Compare the count with \(\varphi(p-1)\).
- Build discrete logarithm tables.

## Main discoveries

- Powers modulo \(p\) are periodic.
- Some elements generate all nonzero residues.
- \(\mathbb F_p^\times\) appears to be cyclic.
- Discrete logarithms are easy to define but hard to invert for large \(p\).

## Mathematical shadows

- Fermat's little theorem.
- Cyclic groups.
- Primitive roots.
- Discrete logarithms.

---

# Session 3 — Quadratic residues

## Central question

Which numbers are squares modulo a prime?

## Experiments

- Compute \(\{x^2\mod p:x\in\mathbb F_p\}\).
- Count quadratic residues.
- Visualize residues on a circle.
- Compute the Legendre symbol \(\left(\frac{a}{p}\right)\).
- Test when \(-1\) is a square modulo \(p\).
- Test when \(2\) is a square modulo \(p\).
- Make heatmaps of \(\left(\frac{a}{p}\right)\).

## Main discoveries

- Exactly half of the nonzero residues are squares.
- \(-1\) is a square modulo \(p\) iff \(p\equiv 1\mod 4\).
- \(2\) has a periodic pattern depending on \(p\mod 8\).

## Mathematical shadows

- Legendre symbol.
- Euler's criterion.
- Supplementary laws of quadratic reciprocity.

---

# Session 4 — Quadratic reciprocity as an experimental theorem

## Central question

How are the questions “is \(p\) a square modulo \(q\)?” and “is \(q\) a square modulo \(p\)?” related?

## Experiments

- For odd primes \(p,q\), compute:

\[
\left(\frac{p}{q}\right),\qquad
\left(\frac{q}{p}\right).
\]

- Make a heatmap of \(\left(\frac{p}{q}\right)\).
- Make a heatmap of the product:

\[
\left(\frac{p}{q}\right)\left(\frac{q}{p}\right).
\]

- Color primes according to their value modulo \(4\).
- Ask students to guess the rule.
- Test the rule on many pairs of primes.

## Main discovery

\[
\left(\frac{p}{q}\right)\left(\frac{q}{p}\right)
=
(-1)^{\frac{p-1}{2}\frac{q-1}{2}}.
\]

## Mathematical shadows

- Quadratic reciprocity.
- Symmetry and antisymmetry in arithmetic.
- Reciprocity as an experimentally visible pattern.

---

# Session 5 — Cubic residues and the failure of a naive analogy

## Central question

What changes when we ask for cubes instead of squares?

## Experiments

- Compute cubic residues:

\[
\{x^3\mod p:x\in\mathbb F_p\}.
\]

- Count nonzero cubic residues.
- Compare primes \(p\equiv 1\mod 3\) and \(p\equiv 2\mod 3\).
- Test whether \(2,3,5\) are cubes modulo \(p\).
- Make heatmaps of cubic residue behavior.
- For primes \(p,q\equiv1\mod3\), test whether \(p\) is a cube modulo \(q\) and whether \(q\) is a cube modulo \(p\).

## Main discoveries

- If \(p\equiv 2\mod 3\), every nonzero element is a cube.
- If \(p\equiv 1\mod 3\), exactly one third of the nonzero elements are cubes.
- Cubic reciprocity is not just quadratic reciprocity with the exponent changed from \(2\) to \(3\).
- The naive integer-level pattern is not as clean.

## Mathematical shadows

- Cubic residues.
- Multiplicative characters of order \(3\).
- The need for cube roots of unity.
- Motivation for Eisenstein integers.

---

# Session 6 — Eisenstein integers and cubic reciprocity

## Central question

What is the right number system for cubic reciprocity?

## Experiments

- Plot the Eisenstein lattice:

\[
\mathbb Z[\omega],\qquad \omega^2+\omega+1=0.
\]

- Compute and visualize the norm:

\[
N(a+b\omega)=a^2-ab+b^2.
\]

- Search for Eisenstein primes.
- Compare rational primes:
  - \(3\) ramifies.
  - \(p\equiv2\mod3\) remains prime.
  - \(p\equiv1\mod3\) splits.
- Visualize splitting of primes \(p=a^2-ab+b^2\).
- Return to cubic residues and explain why \(\mathbb Z[\omega]\) is the natural setting.

## Main discoveries

- Cubic reciprocity requires adjoining cube roots of unity.
- The Eisenstein integers form a triangular lattice.
- Rational primes behave differently depending on \(p\mod3\).
- Higher reciprocity laws force us to enlarge the arithmetic universe.

## Mathematical shadows

- Eisenstein integers.
- Norm forms.
- Splitting of primes.
- Cubic reciprocity.
- Algebraic number theory.

---

# Session 7 — Counting solutions over finite fields: lines and conics

## Central question

How many solutions does an equation have over \(\mathbb F_p\)?

## Experiments

Count and visualize solutions of:

\[
x+y=1,
\]

\[
xy=1,
\]

\[
x^2+y^2=1,
\]

\[
x^2+y^2=a,
\]

\[
X^2+Y^2=Z^2.
\]

Then:

- Vary \(p\).
- Plot the number of solutions as a function of \(p\).
- Compare affine and projective counts.
- Visualize solution sets in \(p\times p\) grids.
- Parametrize a conic using slopes.

## Main discoveries

- Lines have predictable point counts.
- Hyperbolas have predictable point counts.
- Nonsingular projective conics over \(\mathbb F_p\) have \(p+1\) points.
- Counting solutions is geometry over finite fields.

## Mathematical shadows

- Finite fields.
- Affine and projective geometry.
- Conics over finite fields.
- First point-counting formulas.

---

# Session 8 — Elliptic curves and a glimpse of the Weil conjectures

## Central question

How does geometry control the number of solutions modulo \(p\)?

## Experiments

- Choose curves:

\[
E:y^2=x^3+ax+b.
\]

- Count points over \(\mathbb F_p\).
- Compute:

\[
a_p=p+1-\#E(\mathbb F_p).
\]

- Plot \(a_p\) as \(p\) varies.
- Plot \(a_p/(2\sqrt p)\).
- Check experimentally:

\[
|a_p|\le 2\sqrt p.
\]

- Compare:
  - Lines.
  - Conics.
  - Singular cubics.
  - Nonsingular elliptic curves.

## Main discoveries

- Curves over \(\mathbb F_p\) tend to have roughly \(p+1\) points.
- For elliptic curves, the error is bounded by \(2\sqrt p\).
- Singular and nonsingular curves behave differently.
- Geometry controls arithmetic data.

## Mathematical shadows

- Hasse's theorem.
- Elliptic curves over finite fields.
- \(L\)-functions.
- Weil conjectures.
- Birch and Swinnerton-Dyer as a future motivation.

---

# Optional alternatives

If the class needs a more playful or computational session, one of the reciprocity or point-counting sessions can be replaced by:

## Alternative A — Polynomial graphs modulo \(p\)

- Plot \(y=f(x)\mod p\).
- Study collisions and value sets.
- Search for permutation polynomials.
- Compare \(x^d\) for different \(d\).

## Alternative B — Polynomial dynamics modulo \(p\)

- Iterate \(x\mapsto x^2+c\mod p\).
- Draw functional graphs.
- Study cycles and trees.

## Alternative C — Collatz and arithmetic dynamics

- Plot trajectories.
- Compute stopping times.
- Search for record-holders.
- Discuss the gap between computation and proof.

## Alternative D — Pascal triangle modulo \(p\)

- Draw Pascal's triangle modulo \(2,3,5\).
- Discover fractals and Lucas's theorem.
