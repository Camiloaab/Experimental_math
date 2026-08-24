# Suggested 6-Session Plan: Experimental Combinatorics

## Module title

**Experimental Combinatorics: Generate, Search, Count, and Discover**

## Guiding theme

This module treats combinatorics as a computational laboratory. Instead of beginning with proofs, students generate finite objects, visualize them, measure statistics, search for patterns, and formulate conjectures.

The guiding idea is:

> Combinatorics becomes experimental when we generate finite worlds, measure them, search them, and discover laws from the data.

---

## Overview of the 6-session arc

1. Random permutations reveal typical finite structure.
2. Catalan objects reveal the same pattern in many worlds.
3. Lattice polygons reveal geometry through counting.
4. Sandpiles reveal global structure from local rules.
5. Ramsey and graph coloring reveal order forced by constraints.
6. Burnside and Pólya reveal counting through symmetry.

In one sentence:

> We experiment with finite objects until hidden laws become visible.

---

# Session 1 — Random Permutations and Sorting Experiments

## Central question

What does a typical permutation look like?

## Experiments

- Generate many random permutations of size \(n\).
- Count fixed points.
- Count cycles.
- Plot cycle length distributions.
- Count inversions.
- Count descents.
- Compute longest increasing subsequence.
- Draw permutation diagrams.
- Run sorting algorithms:
  - bubble sort,
  - insertion sort,
  - merge sort,
  - quicksort.
- Count swaps and comparisons.
- Visualize sorting as bars moving.
- Compare typical and worst-case behavior.

## Natural questions

- How many fixed points does a typical permutation have?
- How many cycles does it have?
- What does its cycle decomposition look like?
- How disordered is a random permutation?
- How many swaps are needed to sort it?
- How long is the longest increasing subsequence?
- Why does sorting behavior vary so much?

## Main discoveries

- Fixed points are approximately Poisson with mean \(1\).
- The probability of no fixed points approaches about \(1/e\).
- The number of cycles grows slowly, about \(\log n\).
- Inversions are concentrated near \(n(n-1)/4\).
- Bubble-sort swaps are exactly inversions.
- The longest increasing subsequence seems to grow like \(2\sqrt n\).

## Mathematical shadows

- Random permutations.
- Derangements.
- Poisson approximation.
- Cycle decompositions.
- Inversions and descents.
- Sorting algorithms.
- Longest increasing subsequence.

## Suggested notebook outputs

- Histograms of fixed points, cycles, inversions, and LIS length.
- Permutation diagrams.
- Sorting animations.
- Empirical scaling plots.

---

# Session 2 — Catalan Objects and Random Trees

## Central question

Why does the same counting sequence appear in many different worlds?

## Experiments

Generate and count:

- balanced parentheses,
- Dyck paths,
- binary trees,
- polygon triangulations,
- noncrossing matchings,
- stack-sortable permutations,
- pattern-avoiding permutations.

Then:

- Count each family for small \(n\).
- Put the counts side by side.
- Build explicit bijections.
- Randomly generate Catalan objects.
- Measure:
  - height of Dyck paths,
  - height of binary trees,
  - number of leaves,
  - degree distributions in triangulations.
- Visualize typical objects.

## Natural questions

- Why do these different objects have the same counts?
- Can we transform one type of object into another?
- What does a random Dyck path look like?
- Are random binary trees balanced?
- How do typical Catalan objects behave as \(n\) grows?

## Main discoveries

The same sequence appears repeatedly:

\[
1,1,2,5,14,42,132,\dots
\]

These are the Catalan numbers:

\[
C_n=\frac{1}{n+1}\binom{2n}{n}.
\]

Random Catalan objects have typical geometric features.

## Mathematical shadows

- Catalan numbers.
- Bijections.
- Recursive structures.
- Dyck paths.
- Binary trees.
- Random trees.
- Brownian excursion as a distant shadow.

## Suggested notebook outputs

- Side-by-side counts of Catalan families.
- Drawings of Dyck paths, trees, triangulations, and noncrossing matchings.
- Random Catalan object statistics.
- Bijection demonstrations.

---

# Session 3 — Lattice Polygons: Pick's Theorem and Ehrhart Experiments

## Central question

Can geometry be discovered by counting lattice points?

## Experiments

### Pick's theorem

- Draw lattice polygons.
- Compute their area.
- Count interior lattice points \(I\).
- Count boundary lattice points \(B\).
- Search for a formula relating \(A,I,B\).
- Generate random lattice polygons and test the formula.

### Ehrhart experiments

- Choose lattice polygons and polytopes:
  - intervals,
  - triangles,
  - squares,
  - simplices,
  - cubes.
- Dilate the shape by \(t=1,2,3,\dots\).
- Count lattice points in \(tP\).
- Fit a polynomial in \(t\).
- Compare degree with dimension.
- Compare leading coefficient with area or volume.
- Count interior lattice points and test reciprocity.

## Natural questions

- Can area be recovered from lattice points?
- Why do boundary points matter?
- What happens when we dilate a polygon?
- Why do the counts seem polynomial?
- What do the coefficients mean?
- Can negative values of a counting polynomial mean anything?

## Main discoveries

Pick's theorem:

\[
A=I+\frac{B}{2}-1.
\]

Ehrhart phenomenon:

\[
L_P(t)=\#(tP\cap \mathbb Z^d)
\]

is often a polynomial in \(t\), whose degree is the dimension of \(P\).

Ehrhart reciprocity suggests that negative evaluations encode interior lattice points.

## Mathematical shadows

- Pick's theorem.
- Ehrhart polynomials.
- Ehrhart reciprocity.
- Lattice polytopes.
- Discrete geometry.

## Suggested notebook outputs

- Random lattice polygon visualizations.
- Tables of \(A,I,B\).
- Polynomial fits for lattice-point counts.
- Plots of \(L_P(t)\) versus \(t\).

---

# Session 4 — Sandpiles and Chip-Firing

## Central question

How can simple local rules create complex global patterns?

## Experiments

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
- Test whether the final stable state depends on firing order.
- Compare chip-firing on different graph structures.

## Natural questions

- Does the order of firing matter?
- Why do complex patterns appear?
- How large are avalanches?
- How does the graph affect the dynamics?
- Can a local rule create fractal-like structure?
- What does recurrence mean experimentally?

## Main discoveries

- Local rules create beautiful global patterns.
- Stabilization does not depend on firing order.
- Avalanches have complex statistics.
- Graph structure controls dynamics.
- The sandpile identity has fractal-like structure.

## Mathematical shadows

- Abelian sandpile model.
- Chip-firing.
- Graph Laplacian.
- Critical groups.
- Recurrent configurations.
- Self-organized criticality.

## Suggested notebook outputs

- Sandpile stabilization animations.
- Avalanche-size histograms.
- Sandpile identity visualizations.
- Comparisons across graphs.

---

# Session 5 — Ramsey and Graph Coloring Experiments

## Central question

How much order is forced by constraints?

## Experiments

### Ramsey experiments

- Randomly color edges of \(K_n\) red/blue.
- Search for monochromatic triangles.
- Estimate how often monochromatic triangles appear.
- Try to find a coloring of \(K_5\) with no monochromatic triangle.
- Try \(K_6\) and fail.
- Search for colorings avoiding small monochromatic cliques.
- Explore \(R(3,3)=6\) experimentally.

### Graph coloring experiments

- Generate graphs.
- Try greedy coloring.
- Compare different vertex orders.
- Search for graphs requiring many colors.
- Count proper colorings of small graphs.
- Guess chromatic polynomials from evaluations.
- Explore deletion-contraction experimentally.
- Generate random graphs \(G(n,p)\) and estimate chromatic number as \(p\) varies.
- Generate planar graphs and try four-coloring them.

## Natural questions

- Can random colorings avoid monochromatic patterns?
- Why does \(K_6\) force a monochromatic triangle?
- How hard is it to color a graph?
- Why does greedy coloring sometimes fail badly?
- Is the number of colorings a polynomial?
- Do planar graphs really seem to need at most four colors?

## Main discoveries

- Disorder eventually forces order.
- Avoiding patterns becomes rapidly difficult.
- Greedy coloring depends strongly on vertex order.
- The number of colorings appears to be polynomial in the number of colors.
- Random graphs show threshold-like behavior.

## Mathematical shadows

- Ramsey theory.
- Monochromatic cliques.
- Chromatic number.
- Chromatic polynomial.
- Deletion-contraction.
- Four-color theorem.
- Probabilistic method.

## Suggested notebook outputs

- Ramsey search visualizations.
- Random edge-coloring statistics.
- Graph coloring animations.
- Chromatic polynomial interpolation tables.
- Chromatic number versus edge probability plots.

---

# Session 6 — Symmetry Counting: Burnside and Pólya by Experiment

## Central question

How do we count objects when symmetric copies are considered the same?

## Experiments

### Burnside by brute force

- Generate all colorings of a necklace with \(n\) beads and \(k\) colors.
- Identify colorings up to rotation.
- Count orbits by brute force.
- Count fixed colorings under each rotation.
- Compare orbit count with average number of fixed points.
- Repeat for bracelets with rotations and reflections.
- Count colorings of cube faces.

### Pólya enumeration

- Compute cycle structures of group elements.
- Compare brute-force enumeration with Pólya formulas.
- Visualize orbits under symmetry groups.
- Study how the count changes with the number of colors.

## Natural questions

- When are two colorings really the same?
- How many essentially different necklaces are there?
- Why does averaging fixed points count orbits?
- How do rotations and reflections change the count?
- Can we count colorings of cube faces without listing them all?

## Main discovery

Burnside's lemma appears experimentally:

\[
\#\text{orbits}
=
\frac{1}{|G|}\sum_{g\in G}\#\operatorname{Fix}(g).
\]

Pólya enumeration systematizes this for colorings and generating functions.

## Mathematical shadows

- Group actions.
- Orbits.
- Stabilizers.
- Fixed points.
- Burnside's lemma.
- Pólya enumeration.
- Cycle index.

## Suggested notebook outputs

- Necklace and bracelet catalogs.
- Orbit representatives.
- Fixed-point count tables.
- Burnside average comparisons.
- Cube coloring examples.

---

# Optional projects

These topics fit the experimental spirit of the module and can become student projects.

## Integer partitions and Young diagrams

- Generate partitions.
- Draw Young diagrams.
- Study random partitions.
- Search for Ramanujan congruences.

## Polyominoes

- Generate all polyominoes with \(n\) squares.
- Count up to symmetry.
- Try tiling rectangles.
- Search for holes.

## Domino tilings

- Count tilings of small boards.
- Discover the mutilated chessboard obstruction.
- Relate tilings to perfect matchings.

## Cellular automata

- Simulate rule 90, rule 30, and rule 110.
- Observe Sierpiński patterns, randomness, and complexity.

## De Bruijn sequences

- Search for cyclic sequences containing all binary words of length \(n\).
- Build De Bruijn graphs.
- Use Eulerian cycles.

## Error-correcting codes

- Generate codewords.
- Add noise.
- Decode.
- Study Hamming distance and sphere-packing.

## Parking functions

- Simulate parking preferences.
- Count successful sequences.
- Compare with tree counts.

## Young tableaux and RSK

- Apply RSK to random permutations.
- Compare permutation statistics with Young diagram shapes.

---

# Summary

The official six-session plan is:

1. **Random permutations and sorting experiments**
2. **Catalan objects and random trees**
3. **Lattice polygons: Pick's theorem and Ehrhart experiments**
4. **Sandpiles and chip-firing**
5. **Ramsey and graph coloring experiments**
6. **Symmetry counting: Burnside and Pólya by experiment**

This plan is strongly experimental: students generate objects, search for patterns, fit formulas, run simulations, and discover combinatorial laws from data.
