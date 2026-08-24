# Topic Backlog: Probability and Probabilistic Thinking

This backlog is for a probability module in an experimental mathematics course. The emphasis is on exploring probabilistic phenomena through simulation, visualization, and computational experiments, while also using probability as a tool to investigate other areas of mathematics.

The guiding idea is:

> Randomness is both an object of study and an instrument for mathematical exploration.

The module can include classical probability, random walks, Monte Carlo methods, random graphs, PageRank, percolation, the Ising model, random tilings, and probabilistic experiments in combinatorics, topology, geometry, and algorithms.

---

## 1. Law of Large Numbers

**Central question:**  
Why do averages stabilize?

**Experiments:**

- Simulate coin flips.
- Simulate dice rolls.
- Simulate Bernoulli, uniform, exponential, and geometric random variables.
- Plot running averages.
- Compare several independent runs.
- Study convergence speed.
- Compare empirical averages with theoretical expectations.

**Patterns to discover:**

- Randomness becomes regular at large scale.
- Sample averages converge to expected values.
- Individual paths fluctuate, but averages stabilize.

---

## 2. Central Limit Theorem

**Central question:**  
Why does the normal distribution appear everywhere?

**Experiments:**

- Sum many independent random variables.
- Try Bernoulli, dice, uniform, exponential, and other distributions.
- Standardize the sums.
- Plot histograms.
- Compare with a normal density.
- Vary the number of summands.
- Study convergence visually.

**Patterns to discover:**

- Many unrelated distributions lead to the same bell curve.
- The normal distribution is an attractor for sums.
- The phenomenon is universal.

---

## 3. Random walks in one dimension

**Central question:**  
How does a randomly moving particle behave?

**Experiments:**

- Simulate simple random walks on \(\mathbb Z\).
- Plot several paths.
- Plot maximum displacement.
- Estimate typical distance from the origin.
- Study return times.
- Estimate probability of returning to zero.
- Study hitting times.

**Patterns to discover:**

- Typical displacement grows like \(\sqrt n\), not like \(n\).
- Random walks fluctuate strongly.
- One-dimensional random walks return often.

---

## 4. Random walks in two and three dimensions

**Central question:**  
Does dimension change random motion?

**Experiments:**

- Simulate random walks on \(\mathbb Z^2\) and \(\mathbb Z^3\).
- Plot paths.
- Estimate probability of returning to the origin.
- Count distinct visited sites.
- Compare dimensions \(1,2,3\).
- Animate the walk.

**Patterns to discover:**

- Dimension changes recurrence.
- Random walks in dimensions \(1\) and \(2\) return often.
- In dimension \(3\), escape becomes possible.

---

## 5. Brownian motion as a scaling limit

**Central question:**  
What happens when random walks are rescaled?

**Experiments:**

- Simulate random walks with smaller and smaller step sizes.
- Rescale time and space.
- Plot limiting-looking paths.
- Compare with Brownian motion simulations.
- Estimate quadratic variation.

**Patterns to discover:**

- Brownian motion emerges from random walks.
- Paths are continuous-looking but extremely rough.
- Space scales like \(\sqrt{\text{time}}\).

---

## 6. Monte Carlo estimation of \(\pi\)

**Central question:**  
Can randomness compute geometry?

**Experiments:**

- Throw random points into a square.
- Count how many land inside a circle.
- Estimate \(\pi\).
- Track convergence.
- Compare different sample sizes.
- Compare with deterministic grids.

**Patterns to discover:**

- Random sampling estimates areas.
- Error decreases slowly, roughly like \(1/\sqrt N\).
- Monte Carlo is simple but noisy.

---

## 7. Monte Carlo integration

**Central question:**  
Can we estimate integrals by random sampling?

**Experiments:**

- Estimate one-dimensional integrals.
- Estimate areas and volumes.
- Estimate high-dimensional integrals.
- Compare grid integration and Monte Carlo integration.
- Explore variance reduction.
- Estimate expectations by simulation.

**Patterns to discover:**

- Monte Carlo methods are useful in high dimensions.
- Error depends mainly on sample size.
- Randomness can beat grids in high-dimensional problems.

---

## 8. High-dimensional geometry by Monte Carlo

**Central question:**  
What does geometry look like in high dimensions?

**Experiments:**

- Estimate the volume of high-dimensional balls.
- Compare the volume of a cube with the volume of the inscribed ball.
- Sample random points in high-dimensional cubes.
- Study distances to the origin.
- Study pairwise distances.
- Study angles between random vectors.

**Patterns to discover:**

- Most of the cube is far from the center.
- Random vectors are almost orthogonal.
- High-dimensional geometry is counterintuitive.
- Probability is the natural way to explore high dimensions.

---

## 9. Buffon's needle

**Central question:**  
Can probability estimate \(\pi\) from a physical experiment?

**Experiments:**

- Simulate dropping a needle on parallel lines.
- Estimate the crossing probability.
- Recover \(\pi\).
- Compare with the circle-area Monte Carlo method.
- Study variance.

**Patterns to discover:**

- Geometry and probability interact.
- \(\pi\) appears in unexpected experiments.
- Random physical experiments can estimate mathematical constants.

---

## 10. Birthday problem

**Central question:**  
Why do coincidences happen earlier than expected?

**Experiments:**

- Simulate birthdays in a room.
- Estimate probability of a shared birthday.
- Vary the number of people.
- Generalize to hash collisions.
- Compare empirical and exact probabilities.

**Patterns to discover:**

- Pairwise comparisons grow quadratically.
- Collisions happen surprisingly early.
- This phenomenon is relevant to cryptography and algorithms.

---

## 11. Coupon collector problem

**Central question:**  
How long does it take to collect all possibilities?

**Experiments:**

- Simulate collecting coupons.
- Track time to completion.
- Repeat many trials.
- Plot the distribution of completion times.
- Compare with \(n\log n\).
- Study the last missing coupon.

**Patterns to discover:**

- The last few coupons dominate the time.
- Expected time is about \(n\log n\).
- Random waiting times can have long tails.

---

## 12. Branching processes

**Central question:**  
When does a random population survive?

**Experiments:**

- Simulate populations where each individual has a random number of children.
- Try different offspring distributions.
- Estimate extinction probability.
- Compare subcritical, critical, and supercritical cases.
- Plot population trees.

**Patterns to discover:**

- There is a survival/extinction threshold.
- Mean offspring number controls the phase transition.
- Critical systems fluctuate strongly.

---

## 13. Markov chains

**Central question:**  
What happens when the future depends only on the present?

**Experiments:**

- Simulate finite Markov chains.
- Compute transition matrices.
- Estimate stationary distributions.
- Compare empirical frequencies with stationary distributions.
- Visualize convergence to equilibrium.
- Study absorbing chains.

**Patterns to discover:**

- Long-term behavior can become independent of the initial state.
- Stationary distributions describe equilibrium.
- Absorbing states model extinction and trapping.

---

## 14. PageRank and random surfing

**Central question:**  
Can random walks rank importance in a network?

**Experiments:**

- Build small directed graphs.
- Simulate a random surfer.
- Estimate visit frequencies.
- Compare with eigenvector computations.
- Add teleportation.
- Study how rankings change when edges are added or removed.
- Compare PageRank with degree centrality.

**Patterns to discover:**

- Random walks on graphs reveal centrality.
- Stationary distributions can rank nodes.
- Teleportation prevents trapping.
- Probability becomes an algorithm.

---

## 15. Mixing and shuffling

**Central question:**  
How long does it take randomness to forget where it started?

**Experiments:**

- Simulate random walks on cycles, grids, and complete graphs.
- Track distance to equilibrium.
- Simulate card-shuffling models.
- Compare different shuffles.
- Study mixing time experimentally.

**Patterns to discover:**

- Some systems mix quickly, others slowly.
- Geometry controls mixing.
- Randomness can be quantified by convergence to equilibrium.

---

## 16. Erdős-Rényi random graphs

**Central question:**  
What does a random graph look like?

**Experiments:**

- Generate \(G(n,p)\).
- Count edges, components, and isolated vertices.
- Track size of largest component.
- Vary \(p\).
- Study the threshold \(p\sim 1/n\).
- Visualize graphs.
- Study graph diameter and connectivity.

**Patterns to discover:**

- A giant component appears suddenly.
- Connectivity appears suddenly.
- Random graphs undergo phase transitions.
- Local randomness creates global structure.

---

## 17. Random graph coloring and cliques

**Central question:**  
How do difficult combinatorial structures appear randomly?

**Experiments:**

- Generate random graphs.
- Search for cliques.
- Search for independent sets.
- Try greedy coloring.
- Estimate chromatic number heuristically.
- Study thresholds for triangles and other subgraphs.

**Patterns to discover:**

- Random graphs are structured but unpredictable.
- Threshold phenomena occur for subgraphs.
- Probabilistic thinking gives existence results.

---

## 18. Random trees

**Central question:**  
What does a typical tree look like?

**Experiments:**

- Generate random labeled trees using Prüfer codes.
- Compute degree distributions.
- Plot random trees.
- Study diameter and height.
- Compare random trees with paths, stars, and balanced trees.
- Count leaves.

**Patterns to discover:**

- Random trees have many leaves.
- Typical trees are neither path-like nor star-like.
- Prüfer codes give a probabilistic view of Cayley's formula.

---

## 19. Probabilistic method

**Central question:**  
Can randomness prove existence?

**Experiments:**

- Generate random graphs and search for properties.
- Find graphs with no large cliques or independent sets.
- Explore Ramsey-type phenomena.
- Estimate probability that a random object has a desired property.
- Use random search to discover examples.

**Patterns to discover:**

- If a random object has positive probability of having a property, such an object exists.
- Randomness can be used as a proof tool.
- Existence can be shown without explicit construction.

---

## 20. Concentration of measure

**Central question:**  
Why are high-dimensional random quantities often predictable?

**Experiments:**

- Simulate sums of independent random variables.
- Plot deviations from the mean.
- Explore Hoeffding/Chernoff-like behavior experimentally.
- Sample random points in high-dimensional cubes.
- Study distances between random points.
- Estimate volume concentration near the boundary.

**Patterns to discover:**

- High-dimensional randomness is often sharply concentrated.
- Individually noisy variables can collectively be predictable.
- Concentration explains why randomized algorithms work.

---

## 21. Percolation on a grid

**Central question:**  
When does local randomness create global connectivity?

**Experiments:**

- Generate random open/closed sites on a square grid.
- Vary the open probability \(p\).
- Detect whether there is a path from left to right.
- Estimate crossing probability.
- Visualize clusters.
- Study cluster-size distribution.
- Estimate the critical threshold.

**Patterns to discover:**

- There is a sharp phase transition.
- Below critical probability, clusters are small.
- Above critical probability, large spanning clusters appear.
- Critical clusters look fractal.

---

## 22. Bond percolation

**Central question:**  
What changes if edges, rather than vertices, are random?

**Experiments:**

- Randomly keep or delete edges in a grid.
- Study connected components.
- Estimate left-right crossing probability.
- Compare site and bond percolation.
- Explore percolation on different lattices.

**Patterns to discover:**

- The lattice matters.
- Critical thresholds depend on geometry.
- Connectivity emerges suddenly.

---

## 23. Ising model

**Central question:**  
How can local interactions create global order?

**Experiments:**

- Simulate spins \(+1/-1\) on a square grid.
- Use the Metropolis algorithm.
- Vary temperature.
- Visualize spin configurations.
- Measure magnetization.
- Measure energy.
- Compare low, high, and critical temperatures.

**Patterns to discover:**

- Low temperature produces ordered phases.
- High temperature produces disorder.
- Near critical temperature, large-scale clusters appear.
- Local rules create global behavior.

---

## 24. Metropolis algorithm

**Central question:**  
How can we sample from complicated probability distributions?

**Experiments:**

- Use Metropolis to sample simple distributions.
- Apply it to the Ising model.
- Compare accepted and rejected moves.
- Track convergence.
- Study dependence on temperature.
- Visualize Markov-chain sampling.

**Patterns to discover:**

- Markov chains can sample complicated spaces.
- Local random moves can approximate global distributions.
- Sampling is an experimental mathematical tool.

---

## 25. Simulated annealing

**Central question:**  
Can randomness help solve optimization problems?

**Experiments:**

- Optimize a function with many local minima.
- Compare greedy search and simulated annealing.
- Apply to traveling salesman on random points.
- Vary temperature schedules.
- Visualize paths and energies.

**Patterns to discover:**

- Randomness helps escape local minima.
- Cooling schedules matter.
- Optimization can be viewed thermodynamically.

---

## 26. Random matrices

**Central question:**  
What patterns appear in eigenvalues of random matrices?

**Experiments:**

- Generate random symmetric matrices.
- Plot eigenvalue histograms.
- Observe semicircle-law-like behavior.
- Generate random non-symmetric matrices.
- Plot eigenvalues in the complex plane.
- Study spacing between eigenvalues.

**Patterns to discover:**

- Eigenvalues of random matrices have universal behavior.
- Random linear algebra produces rigid patterns.
- Random matrices connect probability, physics, statistics, and number theory.

---

## 27. Random simplicial complexes

**Central question:**  
What does a random topological space look like?

**Experiments:**

- Generate random graphs.
- Build clique complexes.
- Compute connected components.
- Compute cycles.
- Estimate Betti numbers.
- Vary edge probability.
- Plot Betti numbers as a function of \(p\).
- Visualize small complexes.

**Patterns to discover:**

- Topology appears and disappears as randomness changes.
- \(H_0\), \(H_1\), and \(H_2\) have different regimes.
- Random topology has phase transitions.

---

## 28. Random Čech and Vietoris-Rips complexes

**Central question:**  
How does topology emerge from random point clouds?

**Experiments:**

- Sample random points in the plane.
- Build Vietoris-Rips complexes at scale \(r\).
- Compute connected components and cycles.
- Vary \(r\).
- Make barcodes or simple persistence diagrams.
- Compare uniform and clustered point clouds.

**Patterns to discover:**

- Topology depends on scale.
- Persistent homology detects structure.
- Random point clouds have predictable topological phases.

---

## 29. Random walks on groups

**Central question:**  
How does randomness explore algebraic structures?

**Experiments:**

- Random walk on \(\mathbb Z/n\mathbb Z\).
- Random walk on permutation groups.
- Random transpositions in \(S_n\).
- Study how long it takes to become random.
- Compare generating sets.

**Patterns to discover:**

- Algebraic structure affects mixing.
- Random walks can reveal group geometry.
- Shuffling is a random walk on \(S_n\).

---

## 30. Random permutations

**Central question:**  
What does a typical permutation look like?

**Experiments:**

- Generate random permutations.
- Count cycles.
- Plot cycle length distributions.
- Estimate probability of a fixed point.
- Study longest cycle.
- Compare with Poisson predictions.
- Explore derangements.

**Patterns to discover:**

- The number of fixed points is approximately Poisson with mean \(1\).
- Typical permutations have logarithmically many cycles.
- Random combinatorial objects have stable statistics.

---

## 31. Random partitions

**Central question:**  
What does a typical integer partition look like?

**Experiments:**

- Generate random partitions of \(n\).
- Plot Young diagrams.
- Study largest part.
- Study number of parts.
- Compare typical shapes for increasing \(n\).
- Explore limit-shape phenomena.

**Patterns to discover:**

- Random partitions have typical shapes.
- Combinatorial objects can have geometric limits.
- Probability reveals hidden structure in counting problems.

---

## 32. Random tilings and dimer models

**Central question:**  
What patterns emerge from random combinatorial geometry?

**Experiments:**

- Generate domino tilings of small regions.
- Randomly sample tilings.
- Study random tilings of rectangles.
- Study random tilings of Aztec diamonds.
- Visualize many random tilings.
- Color tiles by orientation.
- Observe frozen and disordered regions.
- Explore height functions.

**Patterns to discover:**

- Random tilings are locally random but globally organized.
- Large random tilings develop deterministic limit shapes.
- Frozen and liquid regions coexist.
- Aztec diamonds suggest the arctic circle phenomenon.

---

## 33. Random fractals

**Central question:**  
How can randomness generate fractal geometry?

**Experiments:**

- Generate random Cantor sets.
- Simulate diffusion-limited aggregation.
- Generate random-walk paths.
- Simulate percolation clusters.
- Estimate fractal dimensions numerically.
- Study scaling laws.

**Patterns to discover:**

- Random processes can produce fractal objects.
- Scaling laws appear experimentally.
- Critical systems often have fractal structure.

---

## 34. Randomized algorithms

**Central question:**  
How can randomness make algorithms faster or simpler?

**Experiments:**

- Randomized quicksort.
- Monte Carlo primality testing.
- Random sampling for graph properties.
- Random walks for approximate counting.
- Compare deterministic and randomized algorithms.

**Patterns to discover:**

- Randomness can simplify algorithms.
- Average behavior may be much better than worst-case behavior.
- Some problems are naturally probabilistic.
