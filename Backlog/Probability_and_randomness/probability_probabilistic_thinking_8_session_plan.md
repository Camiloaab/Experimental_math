# Suggested 8-Session Plan: Probability and Probabilistic Thinking

## Module title

**Probability as a Machine for Discovering Structure**

## Guiding theme

Randomness is both a mathematical phenomenon and an experimental tool. It begins as noise, becomes statistical regularity, turns into an algorithm, and finally creates geometry.

---

## Overview of the 8-session arc

1. Random averages become predictable.
2. Random motion creates diffusion.
3. Random sampling computes geometry.
4. Random graphs create combinatorial structure.
5. Random walks rank networks.
6. Local random connectivity creates phase transitions.
7. Local random interactions create order.
8. Random combinatorics creates emergent geometry.

In one sentence:

> Randomness begins as noise, becomes statistical regularity, turns into an algorithm, and finally creates geometry.

---

# Session 1 — Law of Large Numbers and Central Limit Theorem

## Central question

Why does randomness become predictable at large scale?

## Experiments

- Simulate coin flips and dice rolls.
- Plot running averages.
- Sum many independent random variables.
- Try Bernoulli, uniform, exponential, and dice distributions.
- Standardize sums.
- Plot histograms and compare with a normal curve.
- Compare several independent runs.

## Main discoveries

- Averages stabilize.
- Fluctuations are of size roughly \(1/\sqrt n\).
- Sums of many independent variables tend toward a bell curve.
- Different distributions lead to the same limiting shape.

## Mathematical shadows

- Law of Large Numbers.
- Central Limit Theorem.
- Universality.
- Error scaling.

## Suggested notebook outputs

- Running average plots.
- Histograms of normalized sums.
- Comparison with the normal density.

---

# Session 2 — Random Walks and Diffusion

## Central question

How does a randomly moving particle behave?

## Experiments

- Simulate random walks on \(\mathbb Z\).
- Plot many one-dimensional paths.
- Estimate typical displacement after \(n\) steps.
- Simulate random walks on \(\mathbb Z^2\) and \(\mathbb Z^3\).
- Estimate return probabilities.
- Compare dimensions \(1,2,3\).
- Rescale paths to motivate Brownian motion.

## Main discoveries

- Typical distance grows like \(\sqrt n\), not like \(n\).
- Dimension changes behavior.
- Random walks in dimensions \(1\) and \(2\) return often.
- In dimension \(3\), escape becomes possible.
- Brownian motion appears as a scaling limit.

## Mathematical shadows

- Diffusion.
- Recurrence and transience.
- Brownian motion.
- Scaling limits.

## Suggested notebook outputs

- Random-walk path plots.
- Return probability estimates.
- Displacement versus \(\sqrt n\).
- Rescaled walk paths.

---

# Session 3 — Monte Carlo Methods and High-Dimensional Geometry

## Central question

Can randomness compute geometry?

## Experiments

- Estimate \(\pi\) by throwing random points into a square.
- Estimate areas and volumes by random sampling.
- Estimate integrals using Monte Carlo.
- Compare grid integration with random sampling.
- Estimate volumes of high-dimensional balls.
- Sample random points in high-dimensional cubes.
- Study pairwise distances and angles between random vectors.

## Main discoveries

- Monte Carlo error decreases like \(1/\sqrt N\).
- Random sampling becomes useful in high dimension.
- High-dimensional geometry is counterintuitive.
- Most points in high-dimensional spaces are far from the center.
- Random vectors are almost orthogonal.

## Mathematical shadows

- Monte Carlo integration.
- Curse of dimensionality.
- Concentration of measure.
- High-dimensional geometry.

## Suggested notebook outputs

- Running Monte Carlo estimate of \(\pi\).
- Error versus sample size.
- Volume estimates for high-dimensional balls.
- Histograms of pairwise distances and angles.

---

# Session 4 — Random Graphs and Probabilistic Combinatorics

## Central question

What does a typical graph look like?

## Experiments

- Generate Erdős-Rényi random graphs \(G(n,p)\).
- Vary \(p\).
- Count connected components.
- Track the largest component.
- Count isolated vertices.
- Estimate the connectivity threshold.
- Search for triangles, cliques, and independent sets.
- Try greedy coloring on random graphs.

## Main discoveries

- A giant component appears suddenly.
- Connectivity appears suddenly.
- Threshold phenomena are everywhere.
- Random graphs can prove existence indirectly.
- Local randomness creates global structure.

## Mathematical shadows

- Erdős-Rényi random graphs.
- Giant component phase transition.
- Connectivity threshold.
- Probabilistic method.

## Suggested notebook outputs

- Graph visualizations for different \(p\).
- Largest-component size versus \(p\).
- Number of components versus \(p\).
- Clique and independent-set statistics.

---

# Session 5 — PageRank and Random Walks on Networks

## Central question

Can random motion rank importance?

## Experiments

- Build small directed graphs.
- Simulate a random surfer.
- Count visit frequencies.
- Compare empirical frequencies with matrix computations.
- Add teleportation.
- Study how rankings change when edges are added or removed.
- Compare PageRank with degree centrality.
- Apply the idea to small examples: web pages, citation graphs, social networks, or course-topic graphs.

## Main discoveries

- Random walks on graphs reveal centrality.
- Long-term frequencies can rank nodes.
- Teleportation prevents trapping.
- Probability becomes an algorithm.
- The geometry of a graph determines the flow of attention.

## Mathematical shadows

- Markov chains.
- Stationary distributions.
- Eigenvectors.
- PageRank.
- Network science.

## Suggested notebook outputs

- Directed graph visualizations.
- Empirical random-surfer frequencies.
- PageRank vector.
- Comparison of PageRank and degree centrality.

---

# Session 6 — Percolation

## Central question

When does local randomness create global connectivity?

## Experiments

- Generate site percolation on a square grid.
- Vary the open probability \(p\).
- Detect left-right crossings.
- Estimate crossing probability.
- Visualize connected clusters.
- Study cluster-size distributions.
- Compare site and bond percolation.
- Try different lattices if time permits.

## Main discoveries

- Below a critical probability, clusters are small.
- Above a critical probability, large spanning clusters appear.
- Near the critical point, clusters look fractal.
- A global object emerges from local random choices.

## Mathematical shadows

- Phase transitions.
- Critical probability.
- Percolation theory.
- Random geometry.
- Scaling and criticality.

## Suggested notebook outputs

- Percolation grid visualizations.
- Crossing probability versus \(p\).
- Cluster-size histograms.
- Critical-looking configurations.

---

# Session 7 — Ising Model and Metropolis Sampling

## Central question

How can local interactions create global order?

## Experiments

- Simulate spins \(+1/-1\) on a square grid.
- Define local energy by neighboring spins.
- Use the Metropolis algorithm.
- Vary temperature.
- Visualize configurations.
- Measure magnetization.
- Measure energy.
- Study behavior at low, high, and critical temperatures.
- Compare with percolation clusters.

## Main discoveries

- Low temperature produces ordered phases.
- High temperature produces disorder.
- Near the critical temperature, large clusters appear.
- Local rules can create macroscopic order.
- Sampling itself can be done by a Markov chain.

## Mathematical shadows

- Statistical mechanics.
- Markov-chain Monte Carlo.
- Metropolis algorithm.
- Phase transitions.
- Critical phenomena.

## Suggested notebook outputs

- Spin-grid animations or snapshots.
- Magnetization versus temperature.
- Energy versus temperature.
- Configurations at low, critical, and high temperature.

---

# Session 8 — Random Tilings and Emergent Shapes

## Central question

How can random combinatorial objects create deterministic geometry?

## Experiments

- Generate domino tilings of small regions.
- Study random tilings of rectangles.
- Study random tilings of Aztec diamonds.
- Visualize many random tilings.
- Color tiles by orientation.
- Observe frozen and disordered regions.
- Estimate the boundary between frozen and random zones.
- Explore height functions if students are ready.

## Main discoveries

- Random tilings are locally random but globally organized.
- Large random tilings develop deterministic limit shapes.
- Frozen regions and liquid regions coexist.
- The Aztec diamond suggests the arctic circle phenomenon.
- Combinatorics, probability, and geometry meet.

## Mathematical shadows

- Domino tilings.
- Dimer models.
- Limit shapes.
- Arctic circle theorem.
- Height functions.

## Suggested notebook outputs

- Random domino tilings.
- Aztec diamond tilings.
- Orientation-colored tiling plots.
- Visual evidence of frozen and liquid regions.

---

# Optional alternatives and projects

These topics are excellent but probably too much for the main eight sessions.

## Random simplicial complexes

- Generate random graphs.
- Build clique complexes.
- Compute connected components and cycles.
- Estimate Betti numbers.
- Study topological phase transitions.

## Random matrices

- Generate random symmetric matrices.
- Plot eigenvalue histograms.
- Observe semicircle-law-like behavior.
- Plot eigenvalues of non-symmetric matrices in the complex plane.

## Random permutations

- Generate random permutations.
- Count cycles.
- Study fixed points and derangements.
- Explore Poisson behavior.

## Branching processes

- Simulate random populations.
- Estimate extinction probabilities.
- Discover subcritical, critical, and supercritical regimes.

## Coupon collector and birthday problem

- Explore coincidences and rare-event waiting times.
- Connect to hashing, algorithms, and cryptography.

## Simulated annealing

- Use randomness to solve optimization problems.
- Compare with greedy search.
- Apply to traveling salesman or energy minimization.

## Random Čech and Vietoris-Rips complexes

- Sample random point clouds.
- Build complexes at different scales.
- Compute persistent topological features.

---

# Summary

The core eight-session plan is:

1. **Law of Large Numbers and Central Limit Theorem**
2. **Random Walks and Diffusion**
3. **Monte Carlo Methods and High-Dimensional Geometry**
4. **Random Graphs and Probabilistic Combinatorics**
5. **PageRank and Random Walks on Networks**
6. **Percolation**
7. **Ising Model and Metropolis Sampling**
8. **Random Tilings and Emergent Shapes**

This gives a coherent progression from classical probability to random geometry, algorithms, networks, phase transitions, and emergent structure.
