# Topic Backlog: Prime Numbers and Experimental Mathematics

This backlog is meant for an experimental mathematics course. The emphasis is not on proving theorems first, but on using computation, visualization, and numerical evidence to discover patterns, formulate conjectures, and develop mathematical intuition.

The basic dataset can be the first million primes:

\[
p_1=2,\quad p_2=3,\quad p_3=5,\dots,\quad p_{1,000,000}=15,485,863.
\]

Students can work with:

\[
(p_n),\qquad g_n=p_{n+1}-p_n,\qquad \pi(x)=\#\{p\le x\}.
\]

---

## 1. First contact with the primes

**Central question:**  
How frequent are the primes?

**Possible experiments:**

- Plot the first \(N\) primes.
- Plot \(p_n\) versus \(n\).
- Compare \(p_n\) with \(n\log n\).
- Estimate the millionth prime.
- Measure the relative error of different approximations.

**Related phenomena, conjectures, and theorems:**

- Prime Number Theorem.
- Approximation \(p_n\sim n\log n\).

---

## 2. The prime-counting function

**Central question:**  
How many primes are less than \(x\)?

**Possible experiments:**

- Compute and plot \(\pi(x)\).
- Compare \(\pi(x)\) with \(x/\log x\).
- Compare \(\pi(x)\) with \(\operatorname{Li}(x)\).
- Plot absolute and relative errors.
- Investigate when the approximations start becoming good.

**Related phenomena, conjectures, and theorems:**

- Prime Number Theorem.
- Logarithmic integral.
- Skewes-type phenomena.

---

## 3. Gaps between consecutive primes

**Central question:**  
How far apart are consecutive primes?

**Possible experiments:**

- Compute \(g_n=p_{n+1}-p_n\).
- Make histograms of prime gaps.
- Find the largest gap among the first \(N\) primes.
- Plot the running maximum of prime gaps.
- Compare average gaps with \(\log x\).
- Study normalized gaps \(g_n/\log p_n\).

**Related phenomena, conjectures, and theorems:**

- Twin prime conjecture.
- Polignac's conjecture.
- Cramér model.
- Bounded gaps between primes.

---

## 4. Twin primes and prime constellations

**Central question:**  
What small patterns occur among nearby primes?

**Possible experiments:**

- Count pairs \((p,p+2)\).
- Count pairs \((p,p+4)\).
- Count pairs \((p,p+6)\).
- Search for prime triplets.
- Search for prime quadruplets \((p,p+2,p+6,p+8)\).
- Compare frequencies of different patterns.
- Study which patterns are impossible for modular reasons.

**Related phenomena, conjectures, and theorems:**

- Twin prime conjecture.
- Prime constellations.
- Admissible patterns.

---

## 5. Primes in arithmetic progressions

**Central question:**  
Are the primes uniformly distributed modulo \(q\)?

**Possible experiments:**

- Count primes in each residue class modulo \(3\), \(4\), \(5\), \(7\), \(10\), \(30\).
- Compare residue classes that are coprime to the modulus.
- Plot cumulative counts by residue class.
- Study prime number races, for example \(1 \mod 4\) versus \(3 \mod 4\).
- Observe early biases.

**Related phenomena, conjectures, and theorems:**

- Dirichlet's theorem.
- Equidistribution of primes in arithmetic progressions.
- Chebyshev bias.
- Prime number races.

---

## 6. Last digits of primes

**Central question:**  
Are the possible last digits of primes equally frequent?

**Possible experiments:**

- Count primes ending in \(1,3,7,9\).
- Plot cumulative frequencies.
- Study pairs of consecutive last digits.
- Make a \(4\times4\) transition matrix.
- Compare with a random model.

**Related phenomena, conjectures, and theorems:**

- Modular restrictions.
- Biases between consecutive primes.
- Randomness with arithmetic constraints.

---

## 7. General modular patterns

**Central question:**  
How does the sequence \(p_n \mod q\) behave?

**Possible experiments:**

- Take \(q=3,4,5,6,8,10,12,30\).
- Compute frequencies of residues.
- Compute transitions \(p_n\bmod q \to p_{n+1}\bmod q\).
- Visualize transitions with heatmaps.
- Compare with uniform distribution.

**Related phenomena, conjectures, and theorems:**

- Equidistribution.
- Local biases.
- Random models for the primes.

---

## 8. Goldbach's conjecture

**Central question:**  
Is every even integer greater than \(2\) a sum of two primes?

**Possible experiments:**

- For each even number \(2n\), find a decomposition \(2n=p+q\).
- Count the number of decompositions.
- Plot the Goldbach representation function.
- Identify numbers with unusually many or unusually few representations.
- Study the relation with the factorization of the even number.

**Related phenomena, conjectures, and theorems:**

- Strong Goldbach conjecture.
- Probabilistic heuristics.
- Additive problems about primes.

---

## 9. Sums of three primes

**Central question:**  
Is every sufficiently large odd integer a sum of three primes?

**Possible experiments:**

- Search for representations \(n=p+q+r\).
- Count the number of representations.
- Compare sums of two primes and sums of three primes.
- Study how abundant the representations are.

**Related phenomena, conjectures, and theorems:**

- Weak Goldbach conjecture.
- Vinogradov's theorem.
- Additive methods.

---

## 10. Experimental probability that a number is prime

**Central question:**  
What is the probability that an integer near \(x\) is prime?

**Possible experiments:**

- Choose random integers near \(x\).
- Estimate the proportion that are prime.
- Compare with \(1/\log x\).
- Compare random integers with random odd integers.
- Compare integers coprime to \(2\cdot3\cdot5\cdot7\).

**Related phenomena, conjectures, and theorems:**

- Prime Number Theorem.
- Probabilistic models of primality.
- Sieve heuristics.

---

## 11. The Sieve of Eratosthenes

**Central question:**  
How do composite numbers disappear under sieving?

**Possible experiments:**

- Visualize the sieve up to \(N\).
- Animate the removal of multiples.
- Count how many numbers survive after sieving by primes up to \(z\).
- Compare with \(\prod_{p\le z}(1-1/p)\).
- Color each composite by its smallest prime factor.

**Related phenomena, conjectures, and theorems:**

- Sieve methods.
- Euler products.
- Density of integers not divisible by small primes.

---

## 12. Smallest prime factor

**Central question:**  
What is the first prime that detects that a number is composite?

**Possible experiments:**

- Compute the smallest prime factor of each integer.
- Make histograms.
- Plot \(\operatorname{spf}(n)\).
- Study numbers with large smallest prime factor.
- Compare easy and difficult composites.

**Related phenomena, conjectures, and theorems:**

- Sieves.
- Rough numbers.
- Primality and factorization.

---

## 13. Smooth numbers

**Central question:**  
How often does a number factor completely into small primes?

**Possible experiments:**

- Count \(y\)-smooth numbers up to \(N\).
- Plot the proportion as \(y\) varies.
- Compute the largest prime factor of \(n\).
- Make smoothness heatmaps.
- Compare random integers, powers, and primorials.

**Related phenomena, conjectures, and theorems:**

- Smooth numbers.
- Factoring algorithms.
- Cryptography.

---

## 14. Probability of being coprime

**Central question:**  
What proportion of pairs of integers are coprime?

**Possible experiments:**

- Choose random pairs \((a,b)\).
- Compute the proportion with \(\gcd(a,b)=1\).
- Compare with \(6/\pi^2\).
- Visualize a grid colored by coprimality.
- Estimate \(\pi\) experimentally from coprimality.

**Related phenomena, conjectures, and theorems:**

- Riemann zeta function.
- Euler product.
- Formula \(1/\zeta(2)=6/\pi^2\).

---

## 15. Euler's phi function

**Central question:**  
How many numbers less than \(n\) are coprime to \(n\)?

**Possible experiments:**

- Compute \(\varphi(n)\) for \(n\le N\).
- Plot \(\varphi(n)\).
- Plot \(\varphi(n)/n\).
- Search for numbers where \(\varphi(n)/n\) is very small.
- Relate \(\varphi(n)\) to the prime factorization of \(n\).

**Related phenomena, conjectures, and theorems:**

- Euler's totient function.
- Product over prime divisors.
- Primorials.

---

## 16. The Möbius function

**Central question:**  
Does the Möbius function behave like random noise?

**Possible experiments:**

- Compute \(\mu(n)\).
- Plot the sequence \(\mu(n)\).
- Plot the cumulative sum \(M(x)=\sum_{n\le x}\mu(n)\).
- Compare \(M(x)\) with \(\sqrt{x}\).
- Measure the frequencies of \(-1,0,1\).

**Related phenomena, conjectures, and theorems:**

- Mertens conjecture.
- Riemann Hypothesis.
- Multiplicative randomness.

---

## 17. The Liouville function

**Central question:**  
Does the parity of the number of prime factors look random?

**Possible experiments:**

- Compute \(\lambda(n)=(-1)^{\Omega(n)}\).
- Plot the sequence.
- Plot partial sums.
- Compare with random walks.
- Compare with the Möbius function.

**Related phenomena, conjectures, and theorems:**

- Pólya conjecture.
- Multiplicative functions.
- Arithmetic randomness.

---

## 18. Number of prime factors

**Central question:**  
How many prime factors does a typical integer have?

**Possible experiments:**

- Compute \(\omega(n)\), the number of distinct prime factors.
- Compute \(\Omega(n)\), the number of prime factors counted with multiplicity.
- Make histograms.
- Compare the average with \(\log\log n\).
- Check whether the distribution looks normal.

**Related phenomena, conjectures, and theorems:**

- Erdős-Kac theorem.
- Probability in number theory.
- Semiprimes and highly composite numbers.

---

## 19. Squarefree numbers

**Central question:**  
What proportion of integers have no square factor?

**Possible experiments:**

- Count squarefree numbers up to \(N\).
- Compare the density with \(6/\pi^2\).
- Plot the indicator function of being squarefree.
- Study gaps between squarefree numbers.
- Compare with coprimality.

**Related phenomena, conjectures, and theorems:**

- Möbius function.
- Euler product.
- Density \(6/\pi^2\).

---

## 20. Polynomial prime generators

**Central question:**  
Can polynomials produce many primes?

**Possible experiments:**

- Study \(n^2+n+41\).
- Study \(n^2-n+41\).
- Search for values of \(A\) for which \(n^2+n+A\) produces many primes.
- Observe when composites begin to appear.
- Compare different quadratic polynomials.

**Related phenomena, conjectures, and theorems:**

- Prime-generating polynomials.
- Bunyakovsky conjecture.
- Bateman-Horn heuristics.

---

## 21. Primes of special forms

**Central question:**  
What special families of primes appear?

**Possible experiments:**

- Search for Mersenne primes \(2^p-1\).
- Search for Fermat primes \(2^{2^n}+1\).
- Search for Sophie Germain primes.
- Search for safe primes.
- Search for palindromic primes.
- Search for repunit primes.
- Search for Fibonacci primes.

**Related phenomena, conjectures, and theorems:**

- Mersenne primes.
- Fermat primes.
- Cryptography.
- Open conjectures about infinitude.

---

## 22. Primitive roots

**Central question:**  
When does a number generate all nonzero residues modulo \(p\)?

**Possible experiments:**

- Find primitive roots modulo \(p\).
- Count them and compare with \(\varphi(p-1)\).
- Search for the smallest primitive root modulo \(p\).
- Study when \(2\) is a primitive root.
- Make tables for many primes.

**Related phenomena, conjectures, and theorems:**

- Cyclic groups.
- Artin's conjecture.
- Cryptography.

---

## 23. Ulam spiral

**Central question:**  
What visual patterns appear when we draw the primes?

**Possible experiments:**

- Draw the Ulam spiral.
- Mark the primes.
- Observe diagonal patterns.
- Color by residue modulo \(q\).
- Compare with random points of the same density.

**Related phenomena, conjectures, and theorems:**

- Polynomials that produce primes.
- Visualization of arithmetic structure.
- Apparent randomness.

---

## 24. Random models of the primes

**Central question:**  
To what extent do the primes resemble a random sequence?

**Possible experiments:**

- Create a model where \(n\) is declared prime with probability \(1/\log n\).
- Compare real and simulated prime gaps.
- Compare real and simulated twin-prime counts.
- Compare maximal gaps.
- Add modular restrictions to the model.

**Related phenomena, conjectures, and theorems:**

- Cramér model.
- Probabilistic heuristics.
- Randomness with constraints.

---

## 25. Euler product and the zeta function

**Central question:**  
How do the primes encode the zeta function?

**Possible experiments:**

- Compute \(\zeta(s)=\sum 1/n^s\).
- Compute the product \(\prod_p(1-p^{-s})^{-1}\).
- Compare both for \(s=2,3,4\).
- Estimate \(\zeta(2)\).
- Estimate \(\pi\) using \(\zeta(2)=\pi^2/6\).
- Study the series \(\sum_p 1/p\).

**Related phenomena, conjectures, and theorems:**

- Euler product.
- Zeta function.
- Distribution of primes.
- Riemann Hypothesis.

---

## 26. Arithmetic progressions of primes

**Central question:**  
Are there long arithmetic progressions consisting only of primes?

**Possible experiments:**

- Search for progressions of length \(3\).
- Search for progressions of length \(4\), \(5\), etc.
- Find the longest progression among the first \(N\) primes.
- Study restrictions on the common difference.
- Compare with random data.

**Related phenomena, conjectures, and theorems:**

- Green-Tao theorem.
- Arithmetic progressions.
- Additive structure of the primes.

---

## 27. Primes as sums of two squares

**Central question:**  
Which primes can be written as \(a^2+b^2\)?

**Possible experiments:**

- Test each prime \(p\) to see whether \(p=a^2+b^2\).
- Compare with \(p\bmod 4\).
- Find explicit representations.
- Visualize points on the circle \(a^2+b^2=p\).
- Study uniqueness.

**Related phenomena, conjectures, and theorems:**

- Fermat's theorem on sums of two squares.
- Primes \(1\mod 4\).
- Gaussian integers.

---

## 28. Gaussian primes

**Central question:**  
What do primes look like in the complex plane?

**Possible experiments:**

- Draw Gaussian integers \(a+bi\).
- Mark the Gaussian primes.
- Color by norm \(a^2+b^2\).
- Compare rational primes \(1\mod4\) and \(3\mod4\).
- Relate to sums of two squares.

**Related phenomena, conjectures, and theorems:**

- Gaussian integers.
- Unique factorization.
- Splitting of primes.
- Geometry of numbers.

---

## 29. Digits of primes

**Central question:**  
What decimal patterns appear among primes?

**Possible experiments:**

- Count first digits.
- Count digit sums.
- Search for palindromic primes.
- Search for reversible primes.
- Search for circular primes.
- Search for truncatable primes.
- Compare with random integers.

**Related phenomena, conjectures, and theorems:**

- Base-10 restrictions.
- Benford's law.
- Palindromic primes.
- Base-dependent phenomena.

---

## 30. Primes in short intervals

**Central question:**  
How many primes are there in short intervals?

**Possible experiments:**

- Count primes in intervals \([x,x+H]\).
- Try \(H=10,100,1000,\log x,\sqrt{x}\).
- Search for intervals without primes.
- Search for intervals unusually rich in primes.
- Compare with the prediction \(H/\log x\).

**Related phenomena, conjectures, and theorems:**

- Primes in short intervals.
- Large gaps.
- Local variability.

---

## 31. Semiprimes and factorization

**Central question:**  
How common are numbers that are products of two primes?

**Possible experiments:**

- Count semiprimes \(n=pq\).
- Compare semiprimes with primes.
- Study semiprimes with large factors.
- Measure difficulty of factorization.
- Simulate RSA-type numbers.

**Related phenomena, conjectures, and theorems:**

- Factorization.
- RSA cryptography.
- Distribution of semiprimes.

---

## 32. Prime chains

**Central question:**  
How long can a rule that produces new primes survive?

**Possible experiments:**

- Study chains \(p,2p+1,2(2p+1)+1,\dots\).
- Search for Cunningham chains.
- Search for Sophie Germain chains.
- Visualize chains as trees.
- Compare with random predictions.

**Related phenomena, conjectures, and theorems:**

- Sophie Germain primes.
- Safe primes.
- Cunningham chains.

---

## 33. Primes and additive representations

**Central question:**  
In how many ways can a number be represented using primes?

**Possible experiments:**

- Count representations \(n=p+q\).
- Count representations \(n=p+q+r\).
- Study differences \(p-q\).
- Count representations of \(n\) as a sum of several primes.
- Visualize matrices of sums of primes.

**Related phenomena, conjectures, and theorems:**

- Goldbach.
- Additive number theory.
- Circle method.

---

## 34. Primes and elliptic curves

**Central question:**  
What patterns appear when counting points modulo primes?

**Possible experiments:**

- Choose a curve \(E: y^2=x^3+ax+b\).
- Count points of \(E\) modulo different primes \(p\).
- Compute \(a_p=p+1-\#E(\mathbb F_p)\).
- Plot \(a_p\).
- Compare with the Hasse interval \(|a_p|\le 2\sqrt p\).
- Study curves with special behavior.

**Related phenomena, conjectures, and theorems:**

- Elliptic curves over finite fields.
- Hasse's theorem.
- Birch and Swinnerton-Dyer conjecture.
- \(L\)-functions.

---

## 35. Primes and counting solutions modulo \(p\)

**Central question:**  
How does the number of solutions of an equation change as the prime \(p\) varies?

**Possible experiments:**

- Count solutions of \(x^2+y^2=1\mod p\).
- Count solutions of \(y^2=f(x)\mod p\).
- Count solutions of simple systems modulo \(p\).
- Plot the number of solutions as a function of \(p\).
- Compare with approximate predictions.

**Related phenomena, conjectures, and theorems:**

- Geometry over finite fields.
- Local zeta functions.
- Weil conjectures.

---

## 36. Philosophical questions for the module

**Central question:**  
What do we learn by experimenting with primes?

**Discussion questions:**

- When does a graph suggest a conjecture?
- When can a graph be misleading?
- What does it mean for primes to “look random”?
- What structural restrictions prevent them from being truly random?
- Which examples show that checking many cases is not enough?
- Which examples show that experimentation can lead to deep mathematics?

**Related phenomena, conjectures, and theorems:**

- Mertens conjecture.
- Birch and Swinnerton-Dyer conjecture.
- Riemann Hypothesis.
- Goldbach conjecture.
- Twin prime conjecture.
- Green-Tao theorem.
