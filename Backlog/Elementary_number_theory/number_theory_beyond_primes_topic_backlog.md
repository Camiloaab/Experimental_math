# Topic Backlog: Elementary Number Theory Beyond Primes

This backlog is for the second number-theory module of an experimental mathematics course. The emphasis is on modular arithmetic, finite fields, reciprocity laws, arithmetic dynamics, and point counting.

The guiding idea is:

> Modular arithmetic turns arithmetic into finite experimental worlds. In these worlds we can draw, count, iterate, and discover patterns that lead naturally to algebra, geometry, dynamics, reciprocity laws, and the first hints of the Weil conjectures.

---

## 1. Modular arithmetic as a finite universe

**Central question:**  
What does arithmetic look like when numbers wrap around?

**Experiments:**

- Build addition tables modulo \(n\).
- Build multiplication tables modulo \(n\).
- Visualize tables as heatmaps.
- Compare prime moduli and composite moduli.
- Identify units modulo \(n\).
- Identify zero divisors.
- Plot maps such as \(x\mapsto ax\mod n\).

**Patterns to discover:**

- Prime moduli behave like fields.
- Composite moduli have zero divisors.
- Arithmetic modulo \(n\) creates finite algebraic worlds.

---

## 2. Units and Euler's phi function

**Central question:**  
Which numbers have multiplicative inverses modulo \(n\)?

**Experiments:**

- Compute all units modulo \(n\).
- Count them and compare with \(\varphi(n)\).
- Plot \(\varphi(n)\).
- Plot \(\varphi(n)/n\).
- Highlight numbers where \(\varphi(n)/n\) is small.
- Build multiplication tables for the unit group.

**Patterns to discover:**

- \(a\) is invertible modulo \(n\) iff \(\gcd(a,n)=1\).
- The units modulo \(n\) form a finite group.
- Products of many small primes make \(\varphi(n)/n\) small.

---

## 3. Powers, cycles, and Fermat's little theorem

**Central question:**  
What happens when we repeatedly multiply by the same number modulo \(n\)?

**Experiments:**

- Compute \(a,a^2,a^3,\dots\mod n\).
- Find periods.
- Compare prime and composite moduli.
- Test Fermat's little theorem experimentally:

\[
a^{p-1}\equiv 1\mod p.
\]

- Draw cycles of powers modulo \(p\).
- Study orders of elements.

**Patterns to discover:**

- Powers in finite groups are periodic.
- The order of an element divides the size of the group.
- Fermat's little theorem appears naturally.

---

## 4. Primitive roots and discrete logarithms

**Central question:**  
Can one element generate all nonzero residues modulo \(p\)?

**Experiments:**

- Search for primitive roots modulo \(p\).
- Count primitive roots.
- Compare with \(\varphi(p-1)\).
- Compute discrete logarithm tables.
- Visualize the permutation \(k\mapsto g^k\mod p\).
- Compare primitive and non-primitive bases.

**Patterns to discover:**

- \(\mathbb F_p^\times\) is cyclic.
- Primitive roots exist modulo primes.
- Discrete logarithms are easy to define but hard to invert for large primes.

---

## 5. Quadratic residues

**Central question:**  
Which numbers are squares modulo a prime?

**Experiments:**

- Compute \(\{x^2\mod p:x\in\mathbb F_p\}\).
- Count quadratic residues.
- Visualize residues on a circle.
- Compute the Legendre symbol \(\left(\frac{a}{p}\right)\).
- Test whether \(-1\) is a square modulo \(p\).
- Test whether \(2\) is a square modulo \(p\).

**Patterns to discover:**

- Half of the nonzero elements of \(\mathbb F_p\) are squares.
- \(-1\) is a square modulo \(p\) iff \(p\equiv 1\mod 4\).
- The behavior of \(2\) depends on \(p\mod 8\).

---

## 6. Quadratic reciprocity

**Central question:**  
How are the questions “is \(p\) a square modulo \(q\)?” and “is \(q\) a square modulo \(p\)?” related?

**Experiments:**

- For odd primes \(p,q\), compute:

\[
\left(\frac{p}{q}\right),\qquad \left(\frac{q}{p}\right).
\]

- Make a heatmap of \(\left(\frac{p}{q}\right)\).
- Make a heatmap of the product:

\[
\left(\frac{p}{q}\right)\left(\frac{q}{p}\right).
\]

- Color primes by congruence class modulo \(4\).
- Ask students to guess the sign rule.

**Pattern to discover:**

\[
\left(\frac{p}{q}\right)\left(\frac{q}{p}\right)
=
(-1)^{\frac{p-1}{2}\frac{q-1}{2}}.
\]

---

## 7. Cubic residues

**Central question:**  
Which numbers are cubes modulo a prime?

**Experiments:**

- Compute \(\{x^3\mod p:x\in\mathbb F_p\}\).
- Count nonzero cubic residues.
- Compare primes \(p\equiv 1\mod 3\) and \(p\equiv 2\mod 3\).
- Test whether fixed numbers such as \(2,3,5\) are cubes modulo \(p\).
- Make residue heatmaps.
- Compare the map \(x\mapsto x^3\) for different primes.

**Patterns to discover:**

- If \(p\equiv 2\mod 3\), every nonzero element is a cube.
- If \(p\equiv 1\mod 3\), exactly one third of the nonzero elements are cubes.
- The relevant structure is controlled by the group \(\mathbb F_p^\times\).

---

## 8. Cubic reciprocity and Eisenstein integers

**Central question:**  
Why is cubic reciprocity naturally about the Eisenstein integers?

**Experiments:**

- For primes \(p,q\equiv 1\mod 3\), test whether \(p\) is a cube modulo \(q\).
- Test whether \(q\) is a cube modulo \(p\).
- Make cubic-residue reciprocity heatmaps.
- Observe that the pattern is less clean over ordinary integers.
- Plot the Eisenstein lattice:

\[
\mathbb Z[\omega],\qquad \omega^2+\omega+1=0.
\]

- Compute the norm:

\[
N(a+b\omega)=a^2-ab+b^2.
\]

- Visualize Eisenstein primes.
- Observe rational prime behavior:
  - \(3\) ramifies.
  - \(p\equiv 2\mod 3\) remains prime.
  - \(p\equiv 1\mod 3\) splits.

**Patterns to discover:**

- Cubic reciprocity requires adjoining cube roots of unity.
- The correct world is \(\mathbb Z[\omega]\), not just \(\mathbb Z\).
- Higher reciprocity laws often force us to enlarge the number system.

---

## 9. Polynomial graphs modulo \(p\)

**Central question:**  
What do polynomial functions look like over finite fields?

**Experiments:**

- Plot graphs of \(y=f(x)\mod p\).
- Try \(x^2\), \(x^3\), \(x^2+x+1\), \(x^3-x\), \(x^4+x+1\).
- Count how many values are hit.
- Count collisions.
- Study maps \(x\mapsto x^d\).
- Search for permutation polynomials.

**Patterns to discover:**

- Polynomial functions over finite fields are finite maps.
- Some polynomials are permutations.
- \(x\mapsto x^d\) is a permutation of \(\mathbb F_p^\times\) iff \(\gcd(d,p-1)=1\).

---

## 10. Polynomial dynamics modulo \(p\)

**Central question:**  
What happens when we iterate a polynomial modulo \(p\)?

**Experiments:**

- Iterate \(x\mapsto x^2+c\mod p\).
- Iterate \(x\mapsto x^2-1\mod p\).
- Draw functional graphs.
- Identify cycles and trees.
- Compute orbit lengths.
- Compare different primes and different values of \(c\).

**Patterns to discover:**

- Every orbit in a finite set eventually becomes periodic.
- Functional graphs consist of cycles with trees attached.
- Simple polynomial rules can produce complicated finite dynamics.

---

## 11. Collatz and arithmetic dynamics

**Central question:**  
Can a simple deterministic rule produce mysterious global behavior?

**Experiments:**

- Iterate the Collatz map.
- Plot trajectories.
- Compute stopping times.
- Search for record-holders.
- Plot total stopping time for \(n\le N\).
- Study parity sequences.
- Compare with random-walk heuristics.

**Patterns to discover:**

- Every tested orbit seems to reach \(1\).
- Stopping times are highly irregular.
- Experimental evidence can be overwhelming and still not be proof.

---

## 12. Linear congruences and modular geometry

**Central question:**  
What do equations look like in modular grids?

**Experiments:**

- Solve \(ax\equiv b\mod n\).
- Count solutions.
- Visualize \(ax+by\equiv c\mod n\) in an \(n\times n\) grid.
- Compare prime and composite \(n\).
- Draw modular lines.
- Study intersections.

**Patterns to discover:**

- The gcd controls solvability.
- Over \(\mathbb F_p\), linear equations behave like ordinary linear algebra.
- Over composite moduli, zero divisors create strange behavior.

---

## 13. Linear algebra over finite fields

**Central question:**  
What does linear algebra look like over \(\mathbb F_p\)?

**Experiments:**

- Solve systems \(Ax=b\mod p\).
- Compute ranks modulo \(p\).
- Count invertible \(2\times2\) matrices over \(\mathbb F_p\).
- Count lines through the origin in \(\mathbb F_p^2\).
- Count subspaces of \(\mathbb F_p^3\).

**Patterns to discover:**

- Finite vector spaces behave like ordinary vector spaces, but with finite counts.
- The number of lines in \(\mathbb F_p^2\) is \(p+1\).
- Counting linear-algebraic objects gives polynomial formulas in \(p\).

---

## 14. Finite projective geometry

**Central question:**  
What does projective geometry look like over a finite field?

**Experiments:**

- Construct \(\mathbb P^1(\mathbb F_p)\).
- Construct \(\mathbb P^2(\mathbb F_p)\).
- Count points and lines.
- Draw the Fano plane for \(p=2\).
- Build incidence matrices.
- Verify that every two lines meet.

**Patterns to discover:**

- \(\mathbb P^1(\mathbb F_p)\) has \(p+1\) points.
- \(\mathbb P^2(\mathbb F_p)\) has \(p^2+p+1\) points.
- Every projective line has \(p+1\) points.
- The Fano plane is the smallest projective plane.

---

## 15. Counting solutions over finite fields: lines and conics

**Central question:**  
How many solutions does an equation have over \(\mathbb F_p\)?

**Experiments:**

- Count solutions of \(x+y=1\).
- Count solutions of \(xy=1\).
- Count solutions of \(x^2+y^2=1\).
- Count solutions of \(x^2+y^2=a\).
- Count projective solutions of \(X^2+Y^2=Z^2\).
- Visualize solution sets in the \(p\times p\) grid.
- Compare affine and projective counts.

**Patterns to discover:**

- Lines have predictable point counts.
- Hyperbolas have predictable point counts.
- Nonsingular projective conics over \(\mathbb F_p\) have \(p+1\) points.
- Counting solutions is geometry over finite fields.

---

## 16. Fermat curves and diagonal equations

**Central question:**  
How many solutions do equations like \(x^d+y^d=1\) have modulo \(p\)?

**Experiments:**

- Count solutions of \(x^2+y^2=1\).
- Count solutions of \(x^3+y^3=1\).
- Count solutions of \(x^4+y^4=1\).
- Vary \(p\).
- Plot point counts.
- Study dependence on \(p\mod d\).
- Compare affine and projective versions.

**Patterns to discover:**

- Point counts often depend on congruence classes of \(p\).
- Multiplicative characters control the counts.
- Fermat curves lead naturally to Gauss and Jacobi sums.

---

## 17. Elliptic curves over finite fields

**Central question:**  
How many points does an elliptic curve have modulo \(p\)?

**Experiments:**

- Choose curves \(E:y^2=x^3+ax+b\).
- Count points over \(\mathbb F_p\).
- Compute

\[
a_p=p+1-\#E(\mathbb F_p).
\]

- Plot \(a_p\).
- Plot \(a_p/(2\sqrt p)\).
- Check experimentally that \(|a_p|\le 2\sqrt p\).
- Compare different curves.

**Patterns to discover:**

- Elliptic curves have roughly \(p+1\) points modulo \(p\).
- The error is of size about \(\sqrt p\).
- The error contains deep arithmetic information.

---

## 18. A glimpse of the Weil conjectures

**Central question:**  
Why should geometry control point counts over finite fields?

**Experiments:**

- Compare point counts for:
  - A point.
  - The affine line.
  - The projective line.
  - A line.
  - A conic.
  - A singular cubic.
  - A nonsingular elliptic curve.
- Plot \(\#X(\mathbb F_p)\) as \(p\) varies.
- Plot the error from the expected main term.
- Compare singular and nonsingular curves.
- Discuss the role of dimension and genus.

**Patterns to discover:**

- Dimension predicts the main term.
- Geometry controls the error term.
- For curves, \(\#C(\mathbb F_p)\) is often close to \(p+1\).
- The Weil conjectures explain this pattern in vast generality.

---

## 19. Zeta functions of finite varieties

**Central question:**  
Can point counts over finite fields be packaged into a generating function?

**Experiments:**

- Compute \(N_r=\#X(\mathbb F_{p^r})\) for simple examples.
- Formally explore

\[
Z(X,t)=\exp\left(\sum_{r\ge1}N_r\frac{t^r}{r}\right).
\]

- Start with:
  - A point.
  - A finite set.
  - \(\mathbb A^1\).
  - \(\mathbb P^1\).
  - A conic.
  - A simple elliptic curve.

**Patterns to discover:**

- The zeta function is often rational.
- Counts over extensions contain more information than counts over \(\mathbb F_p\) alone.
- This is one gateway to the Weil conjectures.

---

## 20. Pascal triangle modulo \(p\)

**Central question:**  
What patterns appear in binomial coefficients modulo \(p\)?

**Experiments:**

- Draw Pascal's triangle modulo \(2\).
- Draw Pascal's triangle modulo \(3,5,7\).
- Color entries by residue.
- Count nonzero entries.
- Study self-similarity.
- Explore powers of \(p\).

**Patterns to discover:**

- Sierpiński triangle.
- Lucas's theorem.
- Fractals in modular arithmetic.
- Self-similarity from base-\(p\) expansions.

---

## 21. Partitions and Ramanujan congruences

**Central question:**  
What modular patterns appear in the partition function?

**Experiments:**

- Compute \(p(n)\), the number of partitions of \(n\).
- Plot \(p(n)\).
- Study \(p(n)\mod 2,5,7,11\).
- Discover Ramanujan-type congruences:

\[
p(5n+4)\equiv0\mod5.
\]

**Patterns to discover:**

- Partition growth.
- Modular congruences.
- Ramanujan phenomena.
- Generating functions.

---

## 22. Pell equations and continued fractions

**Central question:**  
How do integer solutions to \(x^2-Dy^2=1\) behave?

**Experiments:**

- Compute continued fractions of \(\sqrt D\).
- Observe periodicity.
- Solve Pell equations for small \(D\).
- Plot solutions.
- Compare minimal solutions for different \(D\).

**Patterns to discover:**

- Continued fractions of quadratic irrationals are periodic.
- Pell equations have infinitely many solutions.
- Solutions grow exponentially.

---

## 23. Sum-of-divisors dynamics

**Central question:**  
What happens when we iterate arithmetic functions?

**Experiments:**

- Compute \(\sigma(n)\).
- Iterate \(n\mapsto \sigma(n)-n\).
- Search for perfect numbers.
- Search for amicable pairs.
- Search for aliquot cycles.
- Plot trajectories.

**Patterns to discover:**

- Perfect numbers.
- Amicable numbers.
- Aliquot sequences.
- Arithmetic dynamics.

---

## 24. Waring-type experiments

**Central question:**  
How many powers are needed to represent integers?

**Experiments:**

- Test which numbers are sums of two squares.
- Test which numbers are sums of three squares.
- Test which numbers are sums of four squares.
- Count representations.
- Search for exceptions.
- Study sums of cubes.

**Patterns to discover:**

- Four-square theorem.
- Three-square theorem.
- Local obstructions.
- Waring's problem.
