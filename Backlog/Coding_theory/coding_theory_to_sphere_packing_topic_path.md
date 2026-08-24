# Coding Theory: From Codes to Sphere Packing

This module is for an experimental mathematics course. The goal is to explore coding theory through computation and geometry, not by starting with formal theorems.

## Guiding idea

> Error correction is geometry: messages are points, noise moves points, and good codes are packings of balls.

Students should generate messages, corrupt them, decode them, visualize Hamming space, and discover that error-correcting codes are sphere packings in a finite geometry.

---

## 1. Binary messages as points

**Central question:**  
What is the geometry of binary messages?

**Experiments:**

- Generate binary strings of length \(n\).
- View each string as a point in \(\{0,1\}^n\).
- Visualize the hypercube for \(n=2,3,4\).
- Compute Hamming distances between strings.
- Draw the graph where two strings are connected if they differ in one bit.

**Patterns to discover:**

- Binary strings form a discrete geometric space.
- Hamming distance measures how many bit changes separate two messages.
- The hypercube is the natural geometry of binary communication.

**Mathematical shadows:**

- Hamming distance.
- Hypercube.
- Discrete metric spaces.

---

## 2. Noise as movement in Hamming space

**Central question:**  
What does noise do to a message?

**Experiments:**

- Send a binary string through a noisy channel.
- Flip each bit independently with probability \(p\).
- Measure the Hamming distance between the sent and received strings.
- Repeat many times.
- Plot the distribution of the number of errors.
- Vary \(n\) and \(p\).

**Patterns to discover:**

- Noise moves messages in Hamming space.
- Most received words lie near the original message.
- The number of bit errors is statistically predictable.

**Mathematical shadows:**

- Binary symmetric channel.
- Bernoulli trials.
- Binomial distribution.

---

## 3. Codes as separated point sets

**Central question:**  
How should we choose messages so they can survive noise?

**Experiments:**

- Choose subsets of \(\{0,1\}^n\) as codebooks.
- Compute all pairwise Hamming distances.
- Search for codebooks with large minimum distance.
- Compare random codebooks with structured codebooks.
- Try greedy algorithms for selecting codewords.
- Visualize codewords inside small hypercubes.

**Patterns to discover:**

- Good codes are sets of points far apart from one another.
- Minimum distance controls robustness.
- Increasing distance usually reduces the number of codewords.

**Mathematical shadows:**

- Codebook.
- Minimum distance.
- Code parameters.
- Packing problem.

---

## 4. Decoding as nearest-neighbor search

**Central question:**  
How do we recover the original message after noise?

**Experiments:**

- Pick a codeword.
- Add random bit flips.
- Decode by choosing the nearest codeword.
- Test when decoding succeeds.
- Test when decoding fails.
- Visualize ambiguous regions where two codewords are equally close.
- Compare different codebooks.

**Patterns to discover:**

- Decoding is nearest-neighbor search.
- A code corrects errors when noisy balls around codewords do not overlap.
- If a received word is too far from the original codeword, decoding may fail.

**Mathematical shadows:**

- Nearest-neighbor decoding.
- Voronoi regions in Hamming space.
- Error-correction radius.

---

## 5. Hamming balls

**Central question:**  
How large is the set of words within \(t\) errors of a message?

**Experiments:**

- For a fixed word, list all words at distance \(0,1,2,\dots,t\).
- Count the size of Hamming balls.
- Verify experimentally:

\[
B(n,t)=\sum_{i=0}^{t}\binom{n}{i}.
\]

- Draw balls in small hypercubes.
- Check when balls around codewords overlap.

**Patterns to discover:**

- A Hamming ball consists of all words that can be reached by at most \(t\) bit flips.
- Ball sizes grow combinatorially.
- Error correction is possible only when decoding balls do not overlap.

**Mathematical shadows:**

- Hamming balls.
- Binomial coefficients.
- Sphere packing in the hypercube.

---

## 6. Sphere-packing bound

**Central question:**  
How many codewords can we fit without overlapping error balls?

**Experiments:**

- Choose a code with \(M\) codewords of length \(n\).
- Suppose it corrects \(t\) errors.
- Count the total number of words covered by the \(M\) balls of radius \(t\).
- Compare

\[
M\cdot B(n,t)
\]

with

\[
2^n.
\]

- Try to build codes that come close to filling the whole space.

**Pattern to discover:**

If a binary code of length \(n\) with \(M\) codewords corrects \(t\) errors, then

\[
M\sum_{i=0}^{t}\binom{n}{i}\le 2^n.
\]

**Mathematical shadows:**

- Hamming bound.
- Sphere-packing bound.
- Packing density.
- Code optimality.

---

## 7. Perfect codes

**Central question:**  
Can error balls fill Hamming space exactly?

**Experiments:**

- Search for codes whose decoding balls cover every word exactly once.
- Test small examples.
- Compare repetition codes and Hamming codes.
- Visualize perfect coverage in small cases.
- Count the number of words covered by balls.

**Patterns to discover:**

- Some codes tile Hamming space perfectly.
- Perfect codes are rare and special.
- A perfect code gives optimal use of redundancy.

**Mathematical shadows:**

- Perfect codes.
- Tiling Hamming space.
- Hamming codes.

---

## 8. The \([7,4,3]\) Hamming code

**Central question:**  
Can we build an efficient perfect one-error-correcting code?

**Experiments:**

- Construct the \([7,4,3]\) Hamming code.
- Encode all \(4\)-bit messages into \(7\)-bit codewords.
- Compute all pairwise distances.
- Verify that the minimum distance is \(3\).
- Corrupt each codeword by one bit.
- Decode by nearest neighbor.
- Check that every one-bit error is corrected.
- Count the balls:

\[
16(1+7)=128=2^7.
\]

**Patterns to discover:**

- The \([7,4,3]\) Hamming code corrects one error.
- It has \(16\) codewords.
- The radius-one balls around the codewords exactly fill \(\{0,1\}^7\).
- It is a perfect sphere packing in the hypercube.

**Mathematical shadows:**

- Hamming code.
- Perfect code.
- Linear code.
- Syndrome decoding as an optional extension.

---

## 9. Optional extension: linear codes

**Central question:**  
Can linear algebra build codes?

**Experiments:**

- Work over \(\mathbb F_2\).
- Choose a generator matrix \(G\).
- Encode messages by

\[
c=mG.
\]

- Generate all codewords.
- Compute minimum distance.
- Use a parity-check matrix \(H\).
- Check valid codewords with

\[
Hc^T=0.
\]

**Patterns to discover:**

- Linear subspaces can be used as codes.
- Matrices encode and check messages.
- Linear algebra makes decoding systematic.

**Mathematical shadows:**

- Linear codes.
- Generator matrix.
- Parity-check matrix.
- Syndrome decoding.

---

## 10. Optional extension: Reed-Solomon codes

**Central question:**  
Can polynomials protect information?

**Experiments:**

- Work over a finite field \(\mathbb F_q\).
- Encode a message as coefficients of a polynomial.
- Evaluate the polynomial at several points.
- Erase or corrupt some values.
- Recover the polynomial from enough correct points.

**Patterns to discover:**

- A polynomial is determined by enough points.
- Extra evaluations create redundancy.
- Polynomial interpolation becomes error correction.

**Mathematical shadows:**

- Reed-Solomon codes.
- Finite fields.
- Polynomial interpolation.
- Erasure correction.
