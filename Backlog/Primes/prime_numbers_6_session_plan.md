# Six-Session Plan: Prime Numbers in Experimental Mathematics

This plan is designed for a course in experimental mathematics. The goal is to lead students from natural questions about prime numbers to computational exploration in Jupyter notebooks.

Each session should follow the same general rhythm:

1. Start with a simple natural question.
2. Ask students to guess what should happen.
3. Explore the question computationally.
4. Visualize the data.
5. Formulate one or more conjectures.
6. Reveal the related theorem, conjecture, or open problem.
7. Discuss the limits of experimental evidence.

The course should not try to cover everything about primes. In six sessions, it is better to build a coherent story than to touch too many topics superficially.

---

## Overview of the six-session arc

1. **How many primes are there?**  
   Prime Number Theorem, \(\pi(x)\), \(p_n\), density of primes.

2. **How far apart are primes?**  
   Prime gaps, twin primes, gap statistics, random models.

3. **Where do primes live modulo \(q\)?**  
   Residue classes, Dirichlet's theorem, last digits, prime races.

4. **Can primes add up to everything?**  
   Goldbach's conjecture and additive representations.

5. **How do primes control random integers?**  
   Coprimality, Euler products, \(6/\pi^2\), zeta function.

6. **Do prime factorizations behave randomly?**  
   Möbius function, Liouville function, Mertens function, false conjectures.

This gives a coherent progression:

> primes as a sequence → primes as sparse objects → primes as random-looking objects → primes with modular structure → primes under addition → primes controlling divisibility → primes and multiplicative randomness.

---

# Session 1 — How many primes are there?

## Central question

How frequent are the primes?

## Natural questions for students

- Are primes rare?
- Do they become rarer as numbers get larger?
- Can we predict approximately where the \(n\)-th prime is?
- Can we estimate how many primes there are below \(x\)?
- Is there a simple formula for the density of primes near \(x\)?

## Notebook experiments

- Load or generate the first million primes.
- Plot \(p_n\) versus \(n\).
- Plot \(p_n/n\).
- Compare \(p_n\) with \(n\log n\).
- Compute \(\pi(x)\) for many values of \(x\).
- Compare \(\pi(x)\) with \(x/\log x\).
- Optionally compare \(\pi(x)\) with \(\operatorname{Li}(x)\).
- Plot absolute and relative errors.

## Possible visualizations

- Scatter or line plot of \(p_n\) versus \(n\).
- Plot of \(p_n/(n\log n)\).
- Plot of \(\pi(x)\), \(x/\log x\), and \(\operatorname{Li}(x)\).
- Relative error plots.

## Mathematical shadow

\[
\pi(x)\sim \frac{x}{\log x}.
\]

This is the Prime Number Theorem.

## Pedagogical goal

Students should discover that primes become rarer, but in a surprisingly regular way.

## Possible assignment

Using the first \(N\) primes, estimate the millionth prime using the approximation \(p_n\approx n\log n\). Then compare with the true value.

---

# Session 2 — How far apart are primes?

## Central question

How large are the gaps between consecutive primes?

## Natural questions for students

- Are primes randomly scattered?
- How far apart are consecutive primes?
- What is the most common gap?
- Are there infinitely many pairs of primes separated by \(2\)?
- How large can prime gaps get?
- Does the average gap near \(x\) look like \(\log x\)?

## Notebook experiments

- Compute the prime gaps

\[
g_n=p_{n+1}-p_n.
\]

- Make a histogram of the gaps.
- Plot gaps against \(p_n\).
- Plot the running maximum of the gaps.
- Count twin primes \((p,p+2)\).
- Count cousin primes \((p,p+4)\).
- Count sexy primes \((p,p+6)\).
- Compare the average gap near \(x\) with \(\log x\).
- Study normalized gaps \(g_n/\log p_n\).

## Possible visualizations

- Histogram of prime gaps.
- Scatter plot of \(g_n\) versus \(p_n\).
- Running maximum of prime gaps.
- Cumulative count of twin primes.
- Histogram of normalized gaps.

## Mathematical shadow

- Twin prime conjecture.
- Polignac's conjecture.
- Cramér model.
- Bounded gaps between primes.

## Pedagogical goal

Students should feel that primes look locally irregular, but that this irregularity has statistical structure.

## Possible assignment

Compare the real prime gaps with gaps produced by a random model in which an integer near \(x\) is prime with probability \(1/\log x\).

---

# Session 3 — Where do primes live modulo \(q\)?

## Central question

Are primes uniformly distributed among allowed residue classes?

## Natural questions for students

- Why do primes greater than \(5\) end only in \(1,3,7,9\)?
- Are the last digits \(1,3,7,9\) equally common?
- Are primes evenly distributed modulo \(q\)?
- Does one residue class sometimes lead another?
- Are consecutive last digits of primes random?

## Notebook experiments

- Count primes modulo \(4\), \(6\), \(10\), and \(30\).
- Compare only residue classes coprime to the modulus.
- Plot cumulative counts by residue class.
- Study last digits \(1,3,7,9\).
- Build a \(4\times4\) transition matrix for consecutive last digits.
- Study the race \(1\mod4\) versus \(3\mod4\).
- Optionally study prime races modulo \(3\), \(5\), or \(8\).

## Possible visualizations

- Bar charts of residues modulo \(q\).
- Cumulative count plots for competing residue classes.
- Heatmap of last-digit transitions.
- Prime race plot.

## Mathematical shadow

- Dirichlet's theorem on primes in arithmetic progressions.
- Equidistribution.
- Chebyshev bias.
- Local biases among consecutive primes.

## Pedagogical goal

Students should discover that primes are not simply random points. Modular arithmetic imposes constraints, and even after accounting for those constraints, subtle biases remain.

## Possible assignment

Make a heatmap of transitions \(p_n\bmod q\to p_{n+1}\bmod q\) for \(q=10\) or \(q=30\). Compare it with what a uniform random model would predict.

---

# Session 4 — Can primes add up to everything?

## Central question

Is every even number greater than \(2\) a sum of two primes?

## Natural questions for students

- Can every even number be written as \(p+q\)?
- How many ways can this be done?
- Are some even numbers easier to represent than others?
- Does the number of representations grow?
- Are there even numbers that look dangerously close to being counterexamples?

## Notebook experiments

- For each even number \(2n\), find one Goldbach decomposition.
- Count all decompositions

\[
2n=p+q.
\]

- Plot the Goldbach representation function.
- Identify numbers with unusually many or unusually few representations.
- Study whether divisibility by small primes affects the number of representations.
- Compare the data with a simple probabilistic heuristic.

## Possible visualizations

- Plot of the number of Goldbach representations versus \(2n\).
- Highlight even numbers with many/few representations.
- Scatter plot colored by divisibility properties.
- Matrix visualization of prime sums.

## Mathematical shadow

- Strong Goldbach conjecture.
- Weak Goldbach theorem.
- Additive number theory.
- Heuristics for prime sums.

## Pedagogical goal

Students should see a famous open conjecture as an experimentally very convincing phenomenon, and also understand why convincing numerical evidence is not the same as proof.

## Possible assignment

For even numbers up to \(N\), find the number with the fewest Goldbach representations. Does this minimum grow as \(N\) grows?

---

# Session 5 — How do primes control random integers?

## Central question

What is the probability that two random integers are coprime?

## Natural questions for students

- If we choose two integers randomly, how often do they have no common factor?
- Why should a question about divisibility involve \(\pi\)?
- Can we estimate \(\pi\) experimentally using gcd computations?
- How do primes control divisibility among all integers?

## Notebook experiments

- Generate random pairs \((a,b)\).
- Compute the proportion satisfying \(\gcd(a,b)=1\).
- Compare with

\[
\frac{6}{\pi^2}.
\]

- Draw a grid colored by whether \(\gcd(a,b)=1\).
- Estimate \(\pi\) experimentally from the observed coprimality probability.
- Compute partial Euler products:

\[
\prod_{p\le P}\left(1-\frac{1}{p^2}\right).
\]

- Compare with \(1/\zeta(2)\).

## Possible visualizations

- Coprimality grid.
- Running estimate of the coprimality probability.
- Running estimate of \(\pi\).
- Plot of partial Euler products.

## Mathematical shadow

\[
\mathbb P(\gcd(a,b)=1)=\frac{1}{\zeta(2)}=\frac{6}{\pi^2}.
\]

## Pedagogical goal

Students should see that primes control not only primality but also the statistical behavior of all integers.

## Possible assignment

Estimate \(\pi\) using random coprime pairs. Compare the convergence with a direct Monte Carlo estimate using points in a circle.

---

# Session 6 — Do prime factorizations behave randomly?

## Central question

Does prime factorization produce random-looking arithmetic functions?

## Natural questions for students

- Is the number of prime factors of an integer usually even or odd?
- Does the Möbius function look like random noise?
- Does its cumulative sum behave like a random walk?
- Can a conjecture be supported by enormous numerical evidence and still be false?
- What does this teach us about experimental mathematics?

## Notebook experiments

- Compute the Möbius function \(\mu(n)\).
- Plot the sequence \(\mu(n)\).
- Plot the Mertens function

\[
M(x)=\sum_{n\le x}\mu(n).
\]

- Compare \(M(x)\) with \(\sqrt{x}\).
- Compute the Liouville function

\[
\lambda(n)=(-1)^{\Omega(n)}.
\]

- Plot partial sums of \(\lambda(n)\).
- Compare Möbius and Liouville partial sums with random walks.
- Discuss the false Mertens and Pólya conjectures.

## Possible visualizations

- Sequence plot of \(\mu(n)\).
- Cumulative plot of \(M(x)\).
- Plot of \(M(x)/\sqrt{x}\).
- Sequence and partial sums for \(\lambda(n)\).
- Comparison with simulated random walks.

## Mathematical shadow

- Möbius randomness.
- Mertens conjecture.
- Pólya conjecture.
- Riemann Hypothesis.
- The danger of extrapolating from finite evidence.

## Pedagogical goal

Students should end the prime module with the main philosophical lesson of the course: experiments are powerful tools for discovery, but they are not proofs.

## Possible assignment

Compare the Mertens function with several random walks of the same length. In what ways does it look random? In what ways does it differ?

---

# Optional replacement for Session 6: Visual worlds of primes

If the course needs a more visual ending, Session 6 can be replaced by this topic.

## Central question

What patterns appear when we draw the primes?

## Possible experiments

- Draw the Ulam spiral.
- Color primes by residue class.
- Test which primes are sums of two squares.
- Draw Gaussian primes in the plane.
- Compare visual patterns with modular explanations.

## Mathematical shadow

- Ulam spiral.
- Sums of two squares.
- Gaussian primes.
- Arithmetic structure in visual form.

## Pedagogical goal

Students should see that visualization can reveal hidden arithmetic structure.

---

# Topics to leave for student projects

These are excellent topics, but probably too much for the six core sessions.

- Ulam spiral.
- Gaussian primes.
- Primes as sums of two squares.
- Quadratic residues and reciprocity.
- Primitive roots.
- Carmichael numbers and pseudoprimes.
- Primality testing.
- Smooth numbers.
- Semiprimes and RSA.
- Green-Tao theorem and arithmetic progressions of primes.
- Elliptic curves modulo \(p\).
- Counting solutions modulo primes.
- Prime-generating polynomials.
- Prime chains.
- Digits of primes.
- Primes in short intervals.
