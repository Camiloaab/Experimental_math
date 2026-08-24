# Topic Backlog: Experimental Combinatorics

This backlog is for a combinatorics module in an experimental mathematics course. The emphasis is not on presenting counting theorems abstractly, but on generating finite objects, running searches, visualizing structures, measuring statistics, and discovering patterns experimentally.

The guiding idea is:

> Combinatorics becomes experimental when we generate finite worlds, measure them, search them, and discover laws from the data.

Students should use computation to ask questions such as:

- What does a typical object look like?
- What patterns appear after many trials?
- What changes suddenly when a parameter varies?
- Can we guess a formula from data?
- Can we find counterexamples by search?
- Can we discover a bijection experimentally?
- Can we watch a structure emerge?

---

## 1. Random permutations as a laboratory

**Central question:**  
What does a typical permutation look like?

**Experiments:**

- Generate thousands of random permutations of size \(n\).
- Count fixed points.
- Count cycles.
- Plot cycle length distributions.
- Count inversions.
- Count descents.
- Compute the longest increasing subsequence.
- Draw permutation diagrams.
- Compare empirical distributions as \(n\) grows.

**Patterns to discover:**

- The number of fixed points is usually small.
- The probability of no fixed points approaches about \(1/e\).
- The number of cycles grows slowly, about \(\log n\).
- Inversions are concentrated near \(n(n-1)/4\).
- The longest increasing subsequence seems to grow like \(2\sqrt n\).

**Mathematical shadows:**

- Random permutations.
- Derangements.
- Poisson approximation.
- Cycle decompositions.
- Inversions and descents.
- Longest increasing subsequence.

---

## 2. Sorting as experimental combinatorics

**Central question:**  
How does disorder disappear under sorting?

**Experiments:**

- Generate random permutations.
- Run:
  - bubble sort,
  - insertion sort,
  - merge sort,
  - quicksort.
- Count swaps and comparisons.
- Relate bubble-sort swaps to inversions.
- Visualize sorting as bars moving.
- Compare algorithms statistically over many random permutations.
- Search for worst cases.
- Compare typical and worst-case behavior.

**Patterns to discover:**

- Inversions measure disorder.
- Bubble sort performs one swap per inversion.
- Quicksort has random-looking but predictable behavior.
- Worst-case and typical-case behavior can differ strongly.

**Mathematical shadows:**

- Inversions.
- Algorithmic complexity.
- Average-case analysis.
- Sorting networks and permutation spaces.

---

## 3. Catalan objects as an experimental zoo

**Central question:**  
Why does the same sequence count so many different objects?

**Experiments:**

Generate and count:

- balanced parentheses,
- Dyck paths,
- triangulations of polygons,
- binary trees,
- noncrossing matchings,
- stack-sortable permutations,
- pattern-avoiding permutations.

Then:

- Count objects for small \(n\).
- Put the counts side by side.
- Build explicit bijections.
- Visualize the objects.
- Compare recursion trees.

**Patterns to discover:**

The same sequence appears in many different worlds:

\[
1,1,2,5,14,42,132,\dots
\]

These are the Catalan numbers:

\[
C_n=\frac{1}{n+1}\binom{2n}{n}.
\]

**Mathematical shadows:**

- Catalan numbers.
- Bijections.
- Recursive structures.
- Generating functions.
- Pattern avoidance.

---

## 4. Random Catalan objects

**Central question:**  
What does a typical Catalan object look like?

**Experiments:**

- Generate random Dyck paths of length \(2n\).
- Plot many Dyck paths.
- Measure maximum height.
- Generate random binary trees.
- Measure tree height.
- Generate random triangulations.
- Study degree distributions.
- Generate random noncrossing matchings.
- Compare typical shapes as \(n\) grows.

**Patterns to discover:**

- Random Catalan paths have typical shapes.
- Random Catalan trees are not usually balanced.
- Conditioning a random walk to stay nonnegative produces different geometry.
- Large Catalan objects begin to look probabilistic.

**Mathematical shadows:**

- Random trees.
- Dyck paths.
- Brownian excursion.
- Scaling limits.
- Catalan probability.

---

## 5. Integer partitions as visual experiments

**Central question:**  
How can arithmetic decompositions become geometric objects?

**Experiments:**

- Generate all partitions of \(n\) for small \(n\).
- Draw Young diagrams.
- Generate random partitions of large \(n\).
- Plot typical Young diagrams.
- Compare partitions into odd parts and partitions into distinct parts.
- Compute \(p(n)\mod 5,7,11\).
- Search for Ramanujan congruences experimentally.
- Compare growth of \(p(n)\) with simple exponential functions.

**Patterns to discover:**

- Partition numbers grow very fast.
- Young diagrams turn arithmetic into geometry.
- Partitions into odd parts and distinct parts seem equinumerous.
- Ramanujan congruences appear as surprising modular patterns.
- Random partitions have typical shapes.

**Mathematical shadows:**

- Partition numbers.
- Young diagrams.
- Euler's partition theorem.
- Ramanujan congruences.
- Limit shapes.
- Generating functions.

---

## 6. Random partitions and limit shapes

**Central question:**  
What does a typical partition of a large number look like?

**Experiments:**

- Generate random partitions of \(n\).
- Draw Young diagrams.
- Rescale diagrams.
- Compare many random partitions.
- Estimate typical largest part.
- Estimate typical number of parts.
- Observe emerging limit-shape behavior.

**Patterns to discover:**

- Random partitions have typical macroscopic shapes.
- Large combinatorial objects can become geometric.
- Counting creates probability distributions.

**Mathematical shadows:**

- Limit shapes.
- Asymptotic combinatorics.
- Young diagrams.
- Vershik-Kerov-type phenomena.

---

## 7. Lattice polygons and Pick's theorem

**Central question:**  
Can area be recovered by counting lattice points?

**Experiments:**

- Draw lattice polygons.
- Compute area.
- Count interior lattice points \(I\).
- Count boundary lattice points \(B\).
- Search for a formula relating \(A,I,B\).
- Generate random lattice polygons and test the formula.
- Compare with triangulations into primitive triangles.

**Pattern to discover:**

\[
A=I+\frac{B}{2}-1.
\]

**Mathematical shadows:**

- Pick's theorem.
- Lattice geometry.
- Area from counting.
- Discrete geometry.

---

## 8. Ehrhart experiments

**Central question:**  
How many lattice points are inside a dilated shape?

**Experiments:**

- Choose lattice polygons and polytopes:
  - intervals,
  - triangles,
  - squares,
  - simplices,
  - cubes.
- Count lattice points in \(tP\) for \(t=1,2,3,\dots\).
- Fit a polynomial in \(t\).
- Compare degree with dimension.
- Compare leading coefficient with area or volume.
- Count interior lattice points.
- Test Ehrhart reciprocity.

**Patterns to discover:**

- Lattice-point counts in dilated polytopes are polynomial.
- The degree equals the dimension.
- The leading coefficient is related to volume.
- Negative values of the counting polynomial can encode interior lattice points.

**Mathematical shadows:**

- Ehrhart polynomials.
- Ehrhart reciprocity.
- Pick's theorem.
- Lattice polytopes.

---

## 9. Sandpile model

**Central question:**  
How can simple local rules create complex global patterns?

**Experiments:**

- Put grains of sand on a grid.
- Fire unstable vertices.
- Visualize stabilization.
- Add one grain at a time.
- Study avalanches.
- Track avalanche-size distributions.
- Create the sandpile identity element.
- Try different graphs:
  - path,
  - cycle,
  - grid,
  - complete graph,
  - random graph.

**Patterns to discover:**

- Local rules create beautiful global patterns.
- Stabilization does not depend on firing order.
- Avalanches have complex statistics.
- Graph structure controls dynamics.
- The sandpile identity has fractal-like structure.

**Mathematical shadows:**

- Abelian sandpile model.
- Chip-firing.
- Graph Laplacian.
- Critical groups.
- Self-organized criticality.

---

## 10. Chip-firing on graphs

**Central question:**  
What happens when resources move along edges?

**Experiments:**

- Put chips on graph vertices.
- Fire vertices with enough chips.
- Study stabilization.
- Compare different graphs.
- Compute recurrent states.
- Relate dynamics to spanning trees.
- Visualize firing sequences.
- Test whether stabilization depends on firing order.

**Patterns to discover:**

- Stabilization is independent of firing order.
- Graph structure controls dynamics.
- Chip-firing connects to sandpiles and divisors on graphs.

**Mathematical shadows:**

- Chip-firing games.
- Abelian property.
- Graph Laplacian.
- Divisors on graphs.
- Critical group.

---

## 11. Graph coloring experiments

**Central question:**  
How hard is it to color a graph?

**Experiments:**

- Generate graphs.
- Try greedy coloring.
- Compare different vertex orders.
- Search for graphs requiring many colors.
- Count proper colorings of small graphs.
- Guess chromatic polynomials from evaluations.
- Explore deletion-contraction experimentally.
- Generate random graphs \(G(n,p)\).
- Estimate chromatic number as \(p\) varies.
- Generate planar graphs and try four-coloring them.

**Patterns to discover:**

- Greedy coloring depends strongly on vertex order.
- The number of colorings is a polynomial in the number of colors.
- Some graphs are hard to color.
- Planar graphs seem to need at most four colors.
- Random graphs become harder or easier depending on density.

**Mathematical shadows:**

- Chromatic number.
- Chromatic polynomial.
- Deletion-contraction.
- Four-color theorem.
- Random graphs.

---

## 12. Ramsey experiments

**Central question:**  
How much disorder forces order?

**Experiments:**

- Randomly color edges of \(K_n\) red/blue.
- Search for monochromatic triangles.
- Estimate how often monochromatic triangles appear.
- Try to find a coloring of \(K_5\) with no monochromatic triangle.
- Try \(K_6\) and fail.
- Search computationally for colorings avoiding small monochromatic cliques.
- Explore \(R(3,3)=6\) experimentally.
- Try larger Ramsey-type searches.

**Patterns to discover:**

- Disorder eventually forces order.
- Random colorings almost always contain patterns.
- Avoiding patterns becomes rapidly difficult.
- Small Ramsey numbers can be discovered by exhaustive search.

**Mathematical shadows:**

- Ramsey theory.
- Monochromatic cliques.
- Exhaustive search.
- Probabilistic method.

---

## 13. Burnside's lemma by brute force

**Central question:**  
How do we count objects when symmetric copies are considered the same?

**Experiments:**

- Generate all colorings of a necklace with \(n\) beads and \(k\) colors.
- Identify colorings up to rotation.
- Count orbits by brute force.
- Count fixed colorings under each rotation.
- Compare orbit count with average number of fixed points.
- Repeat for bracelets with rotations and reflections.
- Count colorings of cube faces.

**Pattern to discover:**

\[
\#\text{orbits}
=
\frac{1}{|G|}\sum_{g\in G}\#\operatorname{Fix}(g).
\]

**Mathematical shadows:**

- Burnside's lemma.
- Group actions.
- Orbits.
- Fixed points.
- Symmetry-aware counting.

---

## 14. Pólya enumeration

**Central question:**  
How can symmetry be included in generating functions?

**Experiments:**

- Count colorings of necklaces.
- Count colorings of bracelets.
- Count colorings of cube faces.
- Compare brute-force enumeration with Pólya formulas.
- Compute cycle structures of group elements.
- Visualize orbits under symmetry groups.

**Patterns to discover:**

- Symmetry-aware counting can be systematic.
- Cycle structures of group elements control counts.
- Generating functions can count orbits.

**Mathematical shadows:**

- Pólya enumeration.
- Cycle index.
- Group actions.
- Generating functions with symmetry.

---

## 15. Polyominoes

**Central question:**  
What shapes can be made from unit squares?

**Experiments:**

- Generate all polyominoes with \(n\) squares.
- Count them up to translation, rotation, and reflection.
- Visualize catalogs for small \(n\).
- Try to tile rectangles with a given polyomino.
- Generate random polyominoes.
- Measure perimeter and area.
- Search for holes.
- Compare free, one-sided, and fixed polyomino counts.

**Patterns to discover:**

- Counting grows very fast.
- Symmetry changes the count.
- Some shapes tile rectangles, others do not.
- Typical shapes become irregular.

**Mathematical shadows:**

- Polyomino enumeration.
- Tiling problems.
- Symmetry classes.
- Computational search.

---

## 16. Domino tilings and perfect matchings

**Central question:**  
When can a region be tiled by dominoes?

**Experiments:**

- Tile small rectangles with dominoes.
- Count tilings by brute force.
- Visualize all tilings for small boards.
- Study which boards can be tiled.
- Remove two opposite-colored corners from a chessboard.
- Discover the mutilated chessboard obstruction.
- Represent tilings as perfect matchings in a grid graph.

**Patterns to discover:**

- Coloring arguments give impossibility.
- Tilings correspond to matchings.
- Counts grow exponentially.
- Local constraints create global structure.

**Mathematical shadows:**

- Domino tilings.
- Perfect matchings.
- Bipartite graphs.
- Pfaffian methods.
- Kasteleyn theory.

---

## 17. Cellular automata

**Central question:**  
How can simple local rules create complex behavior?

**Experiments:**

- Simulate elementary cellular automata.
- Try:
  - rule 90,
  - rule 30,
  - rule 110.
- Compare random and structured initial states.
- Study periodicity on finite rings.
- Relate rule 90 to Pascal's triangle modulo \(2\).
- Count patterns over time.

**Patterns to discover:**

- Simple local rules create complexity.
- Some rules are linear and predictable.
- Some rules appear random.
- Pascal/Sierpiński patterns emerge.

**Mathematical shadows:**

- Cellular automata.
- Local rules.
- Sierpiński triangle.
- Computation and complexity.

---

## 18. De Bruijn sequences

**Central question:**  
Can one cyclic sequence contain every possible word exactly once?

**Experiments:**

- Generate binary strings.
- Search for shortest cyclic strings containing every word of length \(n\).
- Build De Bruijn graphs.
- Find Eulerian cycles.
- Generate De Bruijn sequences.
- Visualize word overlaps.

**Patterns to discover:**

- Every word of length \(n\) can appear exactly once in a cyclic sequence.
- The problem becomes finding Eulerian cycles in a graph.
- A string problem transforms into graph theory.

**Mathematical shadows:**

- De Bruijn sequences.
- De Bruijn graphs.
- Eulerian cycles.
- Universal cycles.

---

## 19. Error-correcting codes

**Central question:**  
How can combinatorics protect information from noise?

**Experiments:**

- Generate binary codewords.
- Add random bit flips.
- Try to decode.
- Compute Hamming distances.
- Build repetition codes.
- Build Hamming codes.
- Visualize balls in the hypercube.
- Measure error-correction ability.
- Compare code size, distance, and dimension.

**Patterns to discover:**

- Distance controls error correction.
- Redundancy protects information.
- Sphere-packing bounds appear experimentally.
- Codes are combinatorial geometry in the hypercube.

**Mathematical shadows:**

- Hamming distance.
- Error-correcting codes.
- Sphere-packing bounds.
- Hamming codes.
- Finite geometry.

---

## 20. Parking functions

**Central question:**  
Which preference lists allow everyone to park?

**Experiments:**

- Simulate cars with preferred parking spots.
- Count successful preference sequences.
- Compare with \((n+1)^{n-1}\).
- Generate random parking functions.
- Relate successful sequences to trees.
- Visualize failures and successes.

**Patterns to discover:**

- A simple process gives a rich counting sequence.
- Parking functions connect to trees and Catalan-like structures.
- Local greedy behavior creates global constraints.

**Mathematical shadows:**

- Parking functions.
- Trees.
- Arrangements.
- Catalan combinatorics.

---

## 21. Longest increasing subsequence

**Central question:**  
How long is the longest increasing subsequence of a random permutation?

**Experiments:**

- Generate random permutations.
- Compute LIS length.
- Plot distribution.
- Compare with \(2\sqrt n\).
- Visualize increasing subsequences.
- Compare different values of \(n\).

**Patterns to discover:**

- LIS grows like \(2\sqrt n\).
- Random order has hidden structure.
- A simple statistic leads to deep asymptotics.

**Mathematical shadows:**

- Longest increasing subsequence.
- Random permutations.
- Ulam's problem.
- RSK correspondence.
- Plancherel measure.

---

## 22. Young tableaux and RSK

**Central question:**  
How can permutations turn into shapes?

**Experiments:**

- Generate random permutations.
- Apply RSK.
- Plot resulting Young diagrams.
- Compare shape with longest increasing subsequence.
- Study statistics over many random permutations.
- Compare with random partitions.

**Patterns to discover:**

- Permutations contain hidden partition shapes.
- Longest increasing subsequence becomes geometric.
- Random permutations have limit shapes.

**Mathematical shadows:**

- RSK correspondence.
- Young tableaux.
- Plancherel measure.
- Longest increasing subsequence.
