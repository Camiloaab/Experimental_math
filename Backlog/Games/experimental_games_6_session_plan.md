# Suggested 6-Session Plan: Experimental Games

## Module title

**Games as Experimental Mathematical Laboratories**

## Guiding theme

This module is not meant to be a standard game theory course. Instead, games are treated as simple rule systems that can be simulated, visualized, modified, and used to reveal hidden mathematical structures.

The guiding idea is:

> Take simple games or rules, simulate them, collect statistics, visualize the outcomes, and discover hidden mathematics: stability, fairness, incentives, topology, fixed points, and emergent behavior.

---

## Overview of the 6-session arc

1. Prisoner's dilemma tournaments reveal cooperation and evolution.
2. Rock-paper-scissors reveals cyclic dynamics and coexistence.
3. Gale-Shapley reveals stability, bias, and statistics of matching.
4. Fair division reveals envy, fairness, and efficiency tradeoffs.
5. Auctions reveal how rules shape incentives.
6. Hex and Sperner reveal topology and fixed-point phenomena.

In one sentence:

> Games become laboratories where algorithms, incentives, fairness, dynamics, and topology can be discovered experimentally.

---

# Session 1 — Prisoner's Dilemma Tournaments

## Central question

Which strategies survive in repeated interaction?

## Experiments

- Implement the iterated prisoner's dilemma.
- Create strategies:
  - always cooperate,
  - always defect,
  - tit-for-tat,
  - generous tit-for-tat,
  - grim trigger,
  - random,
  - win-stay lose-shift,
  - copycat with noise.
- Run round-robin tournaments.
- Add noise: sometimes a move is flipped.
- Vary the number of rounds.
- Vary the payoff matrix.
- Let strategies reproduce proportionally to total score.
- Visualize strategy frequencies over generations.

## Natural questions

- Is cooperation stable?
- Does tit-for-tat always win?
- What happens if mistakes happen?
- Can forgiveness help?
- Does evolution favor nice strategies?
- What is the effect of repeated interaction?

## Main discoveries

- Cooperation can emerge without central control.
- Noise makes unforgiving strategies fragile.
- Simple local rules can produce complex population dynamics.
- The best strategy depends on the environment.

## Mathematical shadows

- Iterated games.
- Evolution of cooperation.
- Replicator dynamics.
- Evolutionary stability.
- Agent-based simulation.

## Suggested notebook outputs

- Tournament score tables.
- Heatmap of strategy-versus-strategy performance.
- Strategy frequency plots over generations.
- Comparison of noisy and noiseless tournaments.

---

# Session 2 — Rock-Paper-Scissors and Cyclic Dynamics

## Central question

What happens when strategies beat each other cyclically?

## Experiments

- Simulate rock-paper-scissors.
- Let populations of rock, paper, and scissors reproduce according to payoff.
- Plot frequencies over time.
- Visualize trajectories in the simplex.
- Add mutation.
- Add noise.
- Put agents on a spatial grid.
- Let each cell imitate successful neighbors.
- Watch spiral waves or spatial patterns appear.

## Natural questions

- Why does no strategy take over permanently?
- Do the frequencies settle down?
- Why do cycles appear?
- What changes when agents live on a grid?
- Can diversity be stable?

## Main discoveries

- Nontransitive dominance creates cycles.
- Mixed equilibria can be dynamically unstable, stable, or neutral depending on the update rule.
- Spatial interaction can create beautiful wave patterns.
- Diversity can persist because each strategy has both a predator and a prey.

## Mathematical shadows

- Mixed strategies.
- Replicator dynamics.
- Nontransitive games.
- Population dynamics.
- Cyclic competition.
- Spatial games.

## Suggested notebook outputs

- Frequency plots over time.
- Simplex trajectory plots.
- Spatial grid animations.
- Comparison of well-mixed and spatial populations.

---

# Session 3 — Gale-Shapley as an Experiment in Matching

## Central question

What does stability look like statistically?

## Experiments

- Generate random preference lists for two groups.
- Run the Gale-Shapley deferred acceptance algorithm.
- Compare proposer-optimal and receiver-optimal outcomes.
- Count blocking pairs.
- Measure average rank of assigned partner.
- Measure distribution of ranks.
- Vary number of participants.
- Compare random preferences with structured preferences.
- Introduce incomplete lists.
- Introduce ties.
- Run many trials and collect statistics.

## Natural questions

- Does a stable matching always exist?
- Is the matching fair?
- Who benefits from proposing?
- How often do people get their first choice?
- What happens as the market grows?
- What happens if preferences are correlated?
- What happens if people lie?

## Main discoveries

- Stability is not the same as fairness.
- The proposing side systematically benefits.
- Random matching markets have statistical regularities.
- Small changes in rules change outcomes.
- Algorithms have social consequences.

## Mathematical shadows

- Stable matching.
- Deferred acceptance.
- Blocking pairs.
- Strategy-proofness.
- Market design.
- Statistics of random preferences.

## Suggested notebook outputs

- Histograms of assigned ranks.
- Average proposer versus receiver welfare.
- Statistics across many random markets.
- Examples showing blocking pairs before stabilization.

---

# Session 4 — Fair Division as a Simulation Problem

## Central question

Can simple procedures produce fair outcomes?

## Experiments

### Cake cutting

- Model cake as interval \([0,1]\).
- Give each player a value-density function.
- Simulate cut-and-choose.
- Simulate moving-knife-like procedures.
- Compare:
  - proportionality,
  - envy-freeness,
  - efficiency.
- Visualize each player's subjective value over the cake.

### Indivisible goods

- Generate random valuations for objects.
- Try round-robin picking.
- Try greedy allocation.
- Try maximum total welfare.
- Try envy-minimizing allocation.
- Compute:
  - envy,
  - total welfare,
  - minimum welfare,
  - EF1: envy-free up to one good.
- Compare algorithms over many random valuation profiles.

## Natural questions

- Is equal division fair?
- Can everyone feel they got at least half?
- Can an allocation be efficient but unfair?
- Can an allocation be fair but inefficient?
- What changes when goods are indivisible?
- How often does envy appear?

## Main discoveries

- Fairness depends on preferences.
- Different fairness criteria disagree.
- Indivisible goods make exact fairness difficult.
- Relaxed fairness notions such as EF1 are useful.
- Algorithms expose tradeoffs between fairness and efficiency.

## Mathematical shadows

- Fair division.
- Envy-freeness.
- Proportionality.
- Pareto efficiency.
- EF1.
- Algorithmic fairness.

## Suggested notebook outputs

- Value-density plots for cake cutting.
- Allocation visualizations.
- Envy matrices.
- Fairness-versus-efficiency scatter plots.

---

# Session 5 — Auction Simulations

## Central question

How do rules change incentives?

## Experiments

- Simulate private-value auctions.
- Compare:
  - first-price auctions,
  - second-price auctions,
  - all-pay auctions if desired.
- Generate bidders with random values.
- Test bidding strategies:
  - truthful bidding,
  - bid shading,
  - aggressive bidding,
  - random bidding,
  - learned bidding.
- Measure:
  - seller revenue,
  - winner surplus,
  - efficiency,
  - probability of overpaying.
- Vary number of bidders.
- Simulate common-value auctions.
- Observe winner's curse.

## Natural questions

- Should one bid truthfully?
- Why is second-price special?
- How much should one shade in first-price auctions?
- Does more competition help the seller?
- Can winning be bad news?
- What rules produce better outcomes?

## Main discoveries

- In second-price auctions, truthful bidding is experimentally robust.
- In first-price auctions, bid shading appears naturally.
- More bidders often increase revenue.
- Common-value auctions create the winner's curse.
- Mechanism design is about shaping incentives.

## Mathematical shadows

- Vickrey auction.
- Incentive compatibility.
- Revenue equivalence heuristics.
- Winner's curse.
- Mechanism design.

## Suggested notebook outputs

- Revenue comparisons across auction formats.
- Bid versus value plots.
- Winner surplus histograms.
- Winner's curse simulations.

---

# Session 6 — Hex, Sperner's Lemma, and Fixed Points

## Central question

Can a board game reveal topology?

## Experiments

### Hex

- Implement Hex on \(n\times n\) boards.
- Let students play.
- Simulate random play.
- Detect winners using graph connectivity.
- Verify experimentally that there are no draws.
- Run simple bots:
  - random,
  - greedy connection,
  - blocking,
  - Monte Carlo rollout.
- Study first-player advantage.

### Sperner's lemma

- Triangulate a large triangle.
- Color vertices according to Sperner boundary rules.
- Search for small fully-labeled triangles.
- Randomly generate valid Sperner colorings.
- Count how many trichromatic triangles appear.
- Visualize the path-following proof.

### Fixed-point intuition

- Use Sperner's lemma to motivate Brouwer fixed point theorem.
- Experiment with maps from a triangle to itself.
- Draw displacement vectors.
- Search for approximate fixed points.
- Refine the triangulation and watch the approximation improve.

## Natural questions

- Why can Hex never end in a draw?
- Why must one player have a connecting path?
- What does a board game have to do with topology?
- Why must a Sperner coloring contain a fully labeled small triangle?
- How does this relate to fixed points?
- Can we find fixed points computationally?

## Main discoveries

- Hex is a connectivity game.
- The no-draw property is topological.
- Strategy stealing suggests first-player advantage.
- Sperner's lemma is a discrete fixed-point theorem.
- Brouwer fixed point theorem has a combinatorial shadow.

## Mathematical shadows

- Hex theorem.
- Graph connectivity.
- Strategy stealing.
- Sperner's lemma.
- Brouwer fixed point theorem.
- Discrete topology.

## Suggested notebook outputs

- Hex board visualizations.
- Random-play win statistics.
- Simple Hex bots and tournament results.
- Sperner-colored triangulations.
- Approximate fixed-point visualizations.

---

# Optional projects

These topics fit the spirit of the module and can become student projects.

## Nim and Sprague-Grundy theory

- Compute winning and losing positions.
- Discover xor.
- Compute Grundy numbers for subtraction games.
- Explore nimbers.

## Chomp and strategy stealing

- Solve small boards by dynamic programming.
- Observe first-player wins.
- Compare explicit strategy search with nonconstructive proof.

## Voting systems and social choice

- Generate random voter preferences.
- Compare plurality, Borda, Condorcet, runoff, and approval voting.
- Search for Condorcet cycles.
- Study strategic voting.

## Schelling segregation model

- Put agents on a grid.
- Give them local preferences.
- Move unhappy agents.
- Observe global segregation.

## Multi-armed bandits

- Compare greedy, epsilon-greedy, UCB, and Thompson sampling.
- Track regret.
- Study exploration versus exploitation.

## Minimax games

- Solve tic-tac-toe.
- Compare random, greedy, and minimax agents.
- Visualize game trees.

## Spatial prisoner's dilemma

- Put agents on a grid.
- Let them imitate successful neighbors.
- Observe cooperation clusters.

## Stable roommates

- Generate random preferences.
- Search for stable roommate matchings.
- Compare with Gale-Shapley.

---

# Summary

The official six-session plan is:

1. **Prisoner's dilemma tournaments**
2. **Rock-paper-scissors and cyclic dynamics**
3. **Gale-Shapley statistics**
4. **Fair division experiments**
5. **Auction simulations**
6. **Hex, Sperner's lemma, and fixed points**

This gives a balanced module with strategic interaction, repeated interaction, population dynamics, matching, fairness, incentives, topology, and fixed-point phenomena.
