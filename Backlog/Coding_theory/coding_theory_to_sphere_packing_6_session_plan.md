# Suggested 6-Session Plan: From Codes to Sphere Packing

## Module title

**From Codes to Sphere Packing**

## Guiding idea

Error correction is geometry:

> messages are points, noise moves points, and good codes are packings of balls.

This module is short, visual, and experimental. Students should repeatedly send messages through noise, decode them, measure failure rates, and discover the geometry of Hamming space.

---

# Session 1 — Messages as Points in the Hypercube

## Central question

What is the space of binary messages?

## Experiments

- Generate binary strings of length \(n\).
- View each string as a point in \(\{0,1\}^n\).
- Visualize the hypercube for \(n=2,3,4\).
- Compute Hamming distances.
- Draw edges between strings that differ in one bit.
- Draw Hamming balls of radius \(1\) for small \(n\).

## Main discoveries

- Binary messages form a finite geometric space.
- Hamming distance measures the number of bit changes needed to move from one message to another.
- The hypercube is the natural geometry of binary communication.

## Mathematical shadows

- Hamming distance.
- Hypercube.
- Discrete geometry.

---

# Session 2 — Noise as Movement

## Central question

What does noise do to a message?

## Experiments

- Send binary strings through a noisy channel.
- Flip each bit independently with probability \(p\).
- Measure the Hamming distance between sent and received words.
- Repeat many times.
- Plot the distribution of the number of errors.
- Vary \(n\) and \(p\).
- Compare with the binomial distribution.

## Main discoveries

- Noise moves a point in Hamming space.
- Most received words stay within a predictable radius.
- The number of errors concentrates around \(pn\).

## Mathematical shadows

- Binary symmetric channel.
- Bernoulli trials.
- Binomial distribution.
- Probabilistic noise model.

---

# Session 3 — Codes as Separated Point Sets

## Central question

How should we choose messages so that noise does not confuse them?

## Experiments

- Choose subsets of \(\{0,1\}^n\) as codebooks.
- Compute pairwise Hamming distances.
- Search for codebooks with large minimum distance.
- Compare random and structured codebooks.
- Try greedy construction of codebooks.
- Simulate noisy transmission and test decoding success.

## Main discoveries

- A code is a set of allowed messages.
- Good codewords are far apart.
- Minimum distance controls robustness.
- There is a tradeoff between many codewords and large distance.

## Mathematical shadows

- Codebook.
- Minimum distance.
- Code parameters.
- Packing problem.

---

# Session 4 — Decoding as Nearest-Neighbor Search

## Central question

How can we recover the sent message from a corrupted one?

## Experiments

- Choose a codeword.
- Flip a small number of bits.
- Decode by choosing the nearest codeword.
- Test all errors of radius \(1\), \(2\), etc.
- Visualize when decoding succeeds or fails.
- Identify ambiguous words that are close to two codewords.

## Main discoveries

- Decoding can be interpreted geometrically.
- Each codeword has a decoding region.
- Error correction works when Hamming balls around codewords do not overlap.
- If codewords are at distance \(d\), then the code can correct up to

\[
\left\lfloor \frac{d-1}{2}\right\rfloor
\]

errors.

## Mathematical shadows

- Nearest-neighbor decoding.
- Voronoi regions in Hamming space.
- Error-correction radius.

---

# Session 5 — Hamming Balls and Sphere Packing

## Central question

How many error balls can fit inside the hypercube?

## Experiments

- For a fixed word, count all words within distance \(t\).
- Verify

\[
B(n,t)=\sum_{i=0}^{t}\binom{n}{i}.
\]

- Draw Hamming balls for small \(n\).
- Choose a code with \(M\) codewords.
- Compare

\[
M\cdot B(n,t)
\]

with the total number of words

\[
2^n.
\]

- Try to build large codes whose balls do not overlap.

## Main discoveries

- Error-correcting codes are sphere packings in Hamming space.
- The volume of a Hamming ball limits how many codewords can fit.
- The sphere-packing bound is a geometric obstruction.

## Mathematical shadows

- Hamming balls.
- Sphere-packing bound.
- Hamming bound:

\[
M\sum_{i=0}^{t}\binom{n}{i}\le 2^n.
\]

---

# Session 6 — Perfect Codes and the \([7,4,3]\) Hamming Code

## Central question

Can error balls fill the hypercube exactly?

## Experiments

- Construct the \([7,4,3]\) Hamming code.
- Encode all \(4\)-bit messages into \(7\)-bit codewords.
- Verify that there are \(16\) codewords.
- Compute the minimum distance and check that it is \(3\).
- Corrupt each codeword by one bit.
- Decode by nearest neighbor.
- Verify that all one-bit errors are corrected.
- Count the radius-one balls:

\[
16(1+7)=128=2^7.
\]

## Main discoveries

- The \([7,4,3]\) Hamming code corrects one error.
- The radius-one balls around its codewords do not overlap.
- They also cover the entire space \(\{0,1\}^7\).
- The Hamming code is a perfect sphere packing in the hypercube.

## Mathematical shadows

- Hamming code.
- Perfect code.
- Linear code.
- Syndrome decoding as an optional extension.

---

# Summary

The six-session arc is:

1. **Messages as points in the hypercube**
2. **Noise as movement**
3. **Codes as separated point sets**
4. **Decoding as nearest-neighbor search**
5. **Hamming balls and sphere packing**
6. **Perfect codes and the \([7,4,3]\) Hamming code**

In one sentence:

> Start with binary messages, add noise, separate codewords, decode by nearest neighbor, discover Hamming balls, and end with perfect sphere packings.
