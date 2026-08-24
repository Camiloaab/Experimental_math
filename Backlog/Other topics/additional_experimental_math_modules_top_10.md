# Ten Additional Experimental Mathematics Modules

This list collects ten strong additional modules or mini-modules that could be included in a course on experimental mathematics. Each topic is chosen because students can explore it computationally: by simulation, visualization, random generation, numerical experiments, search, or interactive models.

The guiding criterion is:

> Can students see the phenomenon before proving it?

---

## 1. Chaos and Dynamical Systems

**Guiding idea:**  
Simple deterministic rules can produce periodicity, instability, and chaos.

**Experimental questions:**

- What happens when we iterate the same function many times?
- When do orbits converge to fixed points?
- When do they become periodic?
- When do they become chaotic?
- How can deterministic systems become unpredictable?

**Possible experiments:**

- Iterate maps such as:

\[
x_{n+1}=f(x_n).
\]

- Draw cobweb diagrams.
- Explore the logistic map:

\[
x_{n+1}=rx_n(1-x_n).
\]

- Create bifurcation diagrams.
- Measure sensitivity to initial conditions.
- Estimate Lyapunov exponents.
- Explore period doubling.
- Compare stable, periodic, and chaotic parameter values.

**Phenomena to discover:**

- Attracting and repelling fixed points.
- Periodic orbits.
- Period doubling.
- Chaos.
- Sensitive dependence on initial conditions.
- Bifurcation diagrams.

**Possible notebook outputs:**

- Cobweb diagrams.
- Bifurcation plots.
- Lyapunov exponent plots.
- Orbit visualizations for different parameters.

---

## 2. Fractals and Complex Dynamics

**Guiding idea:**  
Repeated simple rules create infinite complexity and self-similarity.

**Experimental questions:**

- What happens when we iterate functions in the complex plane?
- Why do fractals appear at boundaries between different behaviors?
- How can dimension be non-integer?
- How does local iteration create global geometry?

**Possible experiments:**

- Generate the Mandelbrot set using escape-time iteration.
- Generate Julia sets for different parameters.
- Explore Newton's method as a dynamical system.
- Draw Newton fractals.
- Generate:
  - Cantor set,
  - Sierpiński triangle,
  - Koch curve,
  - Barnsley fern.
- Estimate box-counting dimension.
- Zoom into fractals and observe self-similarity.

**Phenomena to discover:**

- Self-similarity.
- Fractal boundaries.
- Basins of attraction.
- Non-integer dimension.
- Sensitive dependence on initial conditions.

**Possible notebook outputs:**

- Mandelbrot and Julia set images.
- Newton fractals.
- Box-counting dimension estimates.
- Iterated function system animations.

---

## 3. Fourier Analysis, Waves, and Signals

**Guiding idea:**  
Complicated signals can be decomposed into simple waves.

**Experimental questions:**

- How can a complicated function be built from sines and cosines?
- What does frequency mean?
- How can we remove noise from a signal?
- Why do sharp discontinuities create oscillations?

**Possible experiments:**

- Approximate functions by Fourier series.
- Visualize partial sums.
- Explore the Gibbs phenomenon.
- Generate sound waves and musical tones.
- Compute discrete Fourier transforms.
- Filter noise from signals.
- Compress images or audio using frequency components.
- Draw spectrograms.

**Phenomena to discover:**

- Frequency decomposition.
- Fourier series.
- Gibbs phenomenon.
- Noise filtering.
- Signal compression.
- Time-frequency tradeoffs.

**Possible notebook outputs:**

- Fourier approximation animations.
- Frequency spectra.
- Signal denoising examples.
- Image filtering examples.

---

## 4. Optimization Landscapes

**Guiding idea:**  
Algorithms are particles moving through mathematical landscapes.

**Experimental questions:**

- How do algorithms find minima?
- Why do some algorithms get trapped?
- How does step size affect convergence?
- How do local and global minima differ?
- Can randomness help optimization?

**Possible experiments:**

- Run gradient descent on 2D landscapes.
- Visualize paths from many initial points.
- Compare convex and nonconvex functions.
- Explore Newton's method and its basins of attraction.
- Try simulated annealing.
- Try genetic algorithms.
- Run traveling-salesman heuristics.
- Compare greedy search, random search, and annealing.
- Explore constraint satisfaction and SAT experiments.

**Phenomena to discover:**

- Local minima.
- Saddle points.
- Basins of attraction.
- Step-size instability.
- Escaping traps by randomness.
- Optimization versus search.

**Possible notebook outputs:**

- Contour plots with descent paths.
- Basin-of-attraction diagrams.
- Traveling-salesman animations.
- Simulated annealing energy plots.

---

## 5. Spectral Methods and Random Matrices

**Guiding idea:**  
Eigenvectors reveal hidden structure; random matrices reveal universal patterns.

**Experimental questions:**

- What do eigenvectors reveal about data or graphs?
- How can a matrix compress an image?
- What do random eigenvalues look like?
- Can spectra reveal hidden clusters?

**Possible experiments:**

- Use PCA on point clouds.
- Compute SVD of images.
- Reconstruct images using low-rank approximations.
- Compute graph Laplacian eigenvectors.
- Use spectral clustering on graphs.
- Generate random symmetric matrices.
- Plot eigenvalue histograms.
- Generate random non-symmetric matrices and plot eigenvalues in the complex plane.

**Phenomena to discover:**

- Principal directions.
- Low-rank structure.
- Image compression.
- Spectral clustering.
- Semicircle-law-like behavior.
- Circular-law-like behavior.
- Universality.

**Possible notebook outputs:**

- PCA plots.
- Image compression comparisons.
- Spectral clustering visualizations.
- Random matrix eigenvalue plots.

---

## 6. Information, Entropy, and Compression

**Guiding idea:**  
Information is what remains after predictable structure is removed.

**Experimental questions:**

- Why do some files compress better than others?
- How much information is contained in a message?
- What does randomness have to do with incompressibility?
- How can symbol frequencies be exploited?

**Possible experiments:**

- Generate strings from different probability distributions.
- Compute empirical symbol frequencies.
- Estimate Shannon entropy.
- Compare random strings, natural text, repeated text, and structured data.
- Implement run-length encoding.
- Implement Huffman coding.
- Compare fixed-length and variable-length codes.
- Compress text in different languages.
- Study mutual information between variables.

**Phenomena to discover:**

- Entropy.
- Compressibility.
- Prefix codes.
- Huffman coding.
- Random strings are hard to compress.
- Structured data contains redundancy.

**Possible notebook outputs:**

- Frequency histograms.
- Huffman trees.
- Compression-ratio plots.
- Entropy estimates for different sources.

---

## 7. Markets, Bubbles, and Agent-Based Economics

**Guiding idea:**  
Collective economic patterns can emerge from simple individual rules.

**Experimental questions:**

- How do prices form?
- Can markets aggregate information?
- How do bubbles appear?
- How do local rules create global inequality?
- How do strategies interact in markets?

**Possible experiments:**

- Simulate supply and demand.
- Simulate double auctions.
- Create agents with different buying and selling rules.
- Study price discovery.
- Simulate prediction markets.
- Simulate herd behavior.
- Model wealth exchange.
- Explore preferential attachment and “rich get richer” dynamics.
- Compare rational, noisy, and trend-following agents.

**Phenomena to discover:**

- Price discovery.
- Market efficiency and inefficiency.
- Bubbles.
- Herding.
- Wealth concentration.
- Power-law distributions.
- Emergent macro-behavior from micro-rules.

**Possible notebook outputs:**

- Price time series.
- Wealth distribution histograms.
- Agent-based market simulations.
- Bubble and crash scenarios.

---

## 8. Kelly Betting, Risk, and Growth

**Guiding idea:**  
Maximizing expected value is not the same as maximizing long-term growth.

**Experimental questions:**

- How much should one bet when one has an edge?
- Why can positive expected value still lead to ruin?
- What is the difference between average wealth and typical wealth?
- How does risk affect long-term growth?

**Possible experiments:**

- Simulate repeated betting games.
- Compare betting strategies:
  - fixed amount,
  - fixed fraction,
  - all-in,
  - half-Kelly,
  - full Kelly,
  - overbetting.
- Plot wealth trajectories.
- Compare arithmetic mean wealth and median wealth.
- Estimate probability of ruin.
- Vary edge, odds, and volatility.
- Simulate portfolio-like multiplicative growth.

**Phenomena to discover:**

- Expected value versus geometric growth.
- Volatility drag.
- Ruin from overbetting.
- Kelly criterion.
- Difference between ensemble average and time average.
- Risk management.

**Possible notebook outputs:**

- Wealth trajectory simulations.
- Growth-rate curves as a function of bet size.
- Ruin probability plots.
- Comparison of strategies over many trials.

---

## 9. Social Choice, Voting, and Collective Decisions

**Guiding idea:**  
Combining individual preferences into a collective decision is mathematically unstable.

**Experimental questions:**

- How does the voting rule affect the winner?
- How often do voting paradoxes occur?
- Can majority preferences cycle?
- Can strategic voting change the result?
- Why is fair voting difficult?

**Possible experiments:**

- Generate random voter preference rankings.
- Compare voting systems:
  - plurality,
  - runoff,
  - Borda count,
  - Condorcet method,
  - approval voting.
- Search for Condorcet cycles.
- Measure how often different systems choose different winners.
- Test strategic voting.
- Simulate polarization.
- Explore apportionment paradoxes.
- Experiment with gerrymandering on grids.

**Phenomena to discover:**

- Condorcet paradox.
- Majority cycles.
- Voting-system dependence.
- Strategic voting.
- Arrow-style impossibility phenomena.
- Gerrymandering effects.
- Apportionment paradoxes.

**Possible notebook outputs:**

- Voting outcome comparison tables.
- Frequency of paradoxes under random preferences.
- Pairwise majority graphs.
- Gerrymandering maps.

---

## 10. Penrose Tilings, Aperiodic Order, and Quasicrystals

**Guiding idea:**  
Local matching rules can force global nonperiodic order.

**Experimental questions:**

- Can a tiling be ordered but nonperiodic?
- How can local rules prevent periodicity?
- What patterns appear when tiles are repeatedly inflated?
- How does aperiodic order differ from randomness?

**Possible experiments:**

- Generate Penrose tilings by inflation rules.
- Use thick and thin rhombs.
- Visualize matching rules.
- Count tile frequencies.
- Observe convergence to the golden ratio.
- Explore local patches and their repetitions.
- Compare periodic, random, and Penrose tilings.
- Compute approximate diffraction patterns.
- Explore substitution tilings.

**Phenomena to discover:**

- Aperiodicity.
- Local rules forcing global structure.
- Inflation and substitution.
- Golden ratio frequencies.
- Quasicrystal-like order.
- Nonperiodic but nonrandom patterns.

**Possible notebook outputs:**

- Penrose tiling images.
- Inflation animations.
- Tile-frequency plots.
- Patch-frequency experiments.
- Diffraction-like visualizations.

---

# Summary: The 10 Best Additional Experimental Directions

1. **Chaos and Dynamical Systems**
2. **Fractals and Complex Dynamics**
3. **Fourier Analysis, Waves, and Signals**
4. **Optimization Landscapes**
5. **Spectral Methods and Random Matrices**
6. **Information, Entropy, and Compression**
7. **Markets, Bubbles, and Agent-Based Economics**
8. **Kelly Betting, Risk, and Growth**
9. **Social Choice, Voting, and Collective Decisions**
10. **Penrose Tilings, Aperiodic Order, and Quasicrystals**

Together, these topics broaden the course beyond classical mathematics into computation, physics, economics, information, and complex systems while preserving the experimental spirit.
