# Topic Backlog: Experimental Games

This backlog is for a module in an experimental mathematics course. The goal is not to teach a standard game theory course, but to use games as mathematical laboratories.

The guiding idea is:

> Games are simple rule systems where strategies, algorithms, incentives, fairness, topology, and emergent behavior can be explored experimentally.

Students should simulate games, run tournaments, collect statistics, visualize outcomes, change rules, and discover hidden mathematical structures.

---

## 1. Prisoner's dilemma tournaments

**Central question:**  
Which strategies survive in repeated interaction?

**Experiments:**

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

**Questions students can ask:**

- Is cooperation stable?
- Does tit-for-tat always win?
- What happens if mistakes happen?
- Can forgiveness help?
- Does evolution favor nice strategies?
- What is the effect of repeated interaction?

**Patterns to discover:**

- Cooperation can emerge without central control.
- Noise makes unforgiving strategies fragile.
- Simple local rules can produce complex population dynamics.
- The best strategy depends on the environment.

**Mathematical shadows:**

- Iterated games.
- Evolution of cooperation.
- Replicator dynamics.
- Evolutionary stability.
- Agent-based simulation.

---

## 2. Rock-paper-scissors and cyclic dominance

**Central question:**  
What happens when strategies beat each other cyclically?

**Experiments:**

- Simulate rock-paper-scissors.
- Let populations of rock, paper, and scissors reproduce according to payoff.
- Plot frequencies over time.
- Visualize trajectories in the simplex.
- Add mutation.
- Add noise.
- Put agents on a spatial grid.
- Let each cell imitate successful neighbors.
- Watch spiral waves appear.

**Questions students can ask:**

- Why does no strategy take over permanently?
- Do the frequencies settle down?
- Why do cycles appear?
- What changes when agents live on a grid?
- Can diversity be stable?

**Patterns to discover:**

- Nontransitive dominance creates cycles.
- Mixed equilibria can be dynamically unstable, stable, or neutral depending on the rule.
- Spatial interaction can create wave patterns.
- Diversity can persist because each strategy has both a predator and a prey.

**Mathematical shadows:**

- Mixed strategies.
- Replicator dynamics.
- Nontransitive games.
- Population dynamics.
- Cyclic competition.
- Spatial games.

---

## 3. Matching pennies and mixed strategies

**Central question:**  
Why should rational players randomize?

**Experiments:**

- Simulate matching pennies.
- Try deterministic strategies.
- Try biased random strategies.
- Let one player exploit predictable behavior.
- Search for best responses.
- Estimate equilibrium frequencies.
- Visualize payoff as a function of mixed strategy.

**Questions students can ask:**

- What happens if one player becomes predictable?
- Can randomness be optimal?
- What distribution is hardest to exploit?

**Patterns to discover:**

- Predictable strategies can be exploited.
- Randomization can be optimal.
- Mixed equilibria arise naturally.

**Mathematical shadows:**

- Mixed Nash equilibrium.
- Minimax intuition.
- Randomized strategies.

---

## 4. Evolutionary games

**Central question:**  
How do strategies evolve under selection?

**Experiments:**

- Start with a population of strategies.
- Let strategies earn payoffs against random opponents.
- Reproduce strategies proportionally to payoff.
- Simulate replicator dynamics.
- Try:
  - prisoner's dilemma,
  - rock-paper-scissors,
  - hawk-dove,
  - coordination games.
- Plot population frequencies over time.

**Questions students can ask:**

- Which strategies take over?
- Can multiple strategies coexist?
- Can strategy frequencies cycle forever?
- How does noise affect evolution?

**Patterns to discover:**

- Strategy frequencies evolve dynamically.
- Stable equilibria can emerge.
- Cycles and coexistence can occur.
- Success depends on the environment.

**Mathematical shadows:**

- Replicator dynamics.
- Evolutionarily stable strategies.
- Population games.

---

## 5. Spatial games

**Central question:**  
How does geometry affect strategic behavior?

**Experiments:**

- Place agents on a grid.
- Let each agent play prisoner's dilemma with neighbors.
- Let agents imitate successful neighbors.
- Visualize cooperation and defection.
- Vary payoff parameters.
- Add mutation.
- Try rock-paper-scissors on a grid.

**Questions students can ask:**

- Does cooperation survive better on a grid?
- Can clusters protect strategies?
- What patterns appear in spatial rock-paper-scissors?
- How does neighborhood size change the outcome?

**Patterns to discover:**

- Spatial structure can support cooperation.
- Clusters protect strategies.
- Rock-paper-scissors can produce spiral waves.
- Local interaction changes global behavior.

**Mathematical shadows:**

- Cellular automata.
- Spatial evolutionary games.
- Emergent patterns.

---

## 6. Gale-Shapley stable matching

**Central question:**  
What does stability look like statistically?

**Experiments:**

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

**Questions students can ask:**

- Does a stable matching always exist?
- Is the matching fair?
- Who benefits from proposing?
- How often do people get their first choice?
- What happens as the market grows?
- What happens if preferences are correlated?
- What happens if people lie?

**Patterns to discover:**

- Stability is not the same as fairness.
- The proposing side systematically benefits.
- Random matching markets have statistical regularities.
- Small changes in rules change outcomes.
- Algorithms have social consequences.

**Mathematical shadows:**

- Stable matching.
- Deferred acceptance.
- Blocking pairs.
- Strategy-proofness.
- Market design.
- Statistics of random preferences.

---

## 7. Stable roommates problem

**Central question:**  
Does stable matching always exist when everyone belongs to one group?

**Experiments:**

- Generate random preferences among \(n\) agents.
- Search for stable roommate matchings.
- Count how often stable matchings exist.
- Compare with bipartite Gale-Shapley.
- Visualize blocking pairs.
- Study small examples where no stable matching exists.

**Questions students can ask:**

- Why does bipartite matching behave better?
- How often do stable roommate matchings exist?
- What kind of cycles prevent stability?

**Patterns to discover:**

- Stable matchings need not exist.
- Bipartite structure matters.
- Small rule changes can dramatically change the theory.

**Mathematical shadows:**

- Stable roommates.
- Blocking pairs.
- Existence versus nonexistence.

---

## 8. Fair division: cake cutting

**Central question:**  
Can we divide a resource fairly when people value it differently?

**Experiments:**

- Model a cake as the interval \([0,1]\).
- Give agents different value-density functions.
- Simulate cut-and-choose.
- Simulate moving-knife-like procedures.
- Compare:
  - proportionality,
  - envy-freeness,
  - efficiency.
- Visualize each player's subjective value over the cake.
- Add more than two players.

**Questions students can ask:**

- Is equal length the same as equal value?
- Can everyone feel they got a fair share?
- Can fair allocations be inefficient?
- What changes with more players?

**Patterns to discover:**

- Equal pieces need not be equally valuable.
- Fairness depends on preferences.
- Proportionality and envy-freeness are different.
- Procedures matter.

**Mathematical shadows:**

- Fair division.
- Envy-freeness.
- Proportionality.
- Pareto efficiency.

---

## 9. Fair division of indivisible goods

**Central question:**  
How can we divide discrete objects fairly?

**Experiments:**

- Generate random valuations over objects.
- Try round-robin allocation.
- Try greedy allocation.
- Try maximum total value allocation.
- Try envy-minimizing allocation.
- Compute:
  - envy,
  - total welfare,
  - minimum welfare,
  - Pareto efficiency.
- Test EF1: envy-free up to one good.

**Questions students can ask:**

- Why is exact fairness harder for indivisible goods?
- How often does envy appear?
- Can we improve fairness without losing too much efficiency?
- Which algorithms perform well on random instances?

**Patterns to discover:**

- Exact envy-freeness may be impossible.
- Efficiency and fairness can conflict.
- EF1 is often achievable.
- Random preferences reveal typical behavior.

**Mathematical shadows:**

- Algorithmic fair division.
- Envy-freeness.
- EF1.
- Welfare optimization.

---

## 10. Auctions: first-price and second-price

**Central question:**  
How do rules change bidding behavior?

**Experiments:**

- Simulate bidders with private values.
- Compare:
  - first-price auctions,
  - second-price auctions,
  - all-pay auctions.
- Let bidders use different strategies:
  - truthful bidding,
  - bid shading,
  - aggressive bidding,
  - random bidding,
  - learned bidding.
- Estimate:
  - seller revenue,
  - winner surplus,
  - efficiency,
  - probability of overpaying.
- Vary number of bidders.

**Questions students can ask:**

- Should one bid truthfully?
- Why is second-price special?
- How much should one shade in first-price auctions?
- Does more competition help the seller?
- What rules produce better outcomes?

**Patterns to discover:**

- In second-price auctions, truthful bidding is experimentally robust.
- In first-price auctions, bid shading appears naturally.
- More bidders often increase revenue.
- Auction format affects incentives.

**Mathematical shadows:**

- Vickrey auction.
- Incentive compatibility.
- Revenue and efficiency.
- Mechanism design.

---

## 11. Common-value auctions and winner's curse

**Central question:**  
Why can winning be bad news?

**Experiments:**

- Simulate auctions where the item has one common value.
- Give bidders noisy estimates of that value.
- Let bidders bid their estimates.
- Measure winner's profit.
- Vary noise.
- Vary number of bidders.
- Try bid shading.

**Questions students can ask:**

- Why does the winner often overpay?
- What happens when there are more bidders?
- How should bidders adjust for uncertainty?

**Patterns to discover:**

- The highest estimate is usually too optimistic.
- Winners overpay if they ignore selection bias.
- More bidders can worsen the winner's curse.

**Mathematical shadows:**

- Winner's curse.
- Common-value auctions.
- Selection bias.

---

## 12. Voting systems

**Central question:**  
How does the voting rule affect the winner?

**Experiments:**

- Generate random voter preferences.
- Run:
  - plurality,
  - runoff,
  - Borda count,
  - Condorcet method,
  - approval voting.
- Compare winners.
- Search for Condorcet cycles.
- Test sensitivity to strategic voting.
- Measure frequency of paradoxes.

**Questions students can ask:**

- Can different voting systems choose different winners?
- Can majority preferences cycle?
- How often do paradoxes occur?
- Can voters benefit by misreporting?

**Patterns to discover:**

- Different voting systems can choose different winners.
- Majority preferences can cycle.
- No voting system is perfect.
- Social choice is experimentally rich.

**Mathematical shadows:**

- Condorcet paradox.
- Voting theory.
- Social choice.
- Arrow-type impossibility phenomena.

---

## 13. Schelling segregation model

**Central question:**  
Can mild local preferences create strong global patterns?

**Experiments:**

- Put agents of two types on a grid.
- Give each agent a tolerance threshold.
- Move unhappy agents.
- Visualize the grid over time.
- Vary tolerance.
- Measure segregation.
- Compare random initial states.

**Questions students can ask:**

- How strong do preferences need to be to create segregation?
- Does global segregation imply strong individual bias?
- How does geometry affect the result?

**Patterns to discover:**

- Weak local preferences can create strong global patterns.
- Individual incentives need not reflect collective outcomes.
- Spatial games generate emergent structure.

**Mathematical shadows:**

- Agent-based modeling.
- Emergence.
- Spatial dynamics.
- Social simulation.

---

## 14. Hex

**Central question:**  
Can a board game reveal topology?

**Experiments:**

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

**Questions students can ask:**

- Why can Hex never end in a draw?
- Why must one player have a connecting path?
- Why does the first player have an advantage?
- How good are simple Monte Carlo bots?

**Patterns to discover:**

- Hex is a connectivity game.
- The no-draw property is topological.
- Strategy stealing suggests first-player advantage.
- Local moves create global paths.

**Mathematical shadows:**

- Hex theorem.
- Graph connectivity.
- Strategy stealing.
- Discrete topology.

---

## 15. Sperner's lemma

**Central question:**  
Why must some colored triangle be fully labeled?

**Experiments:**

- Triangulate a large triangle.
- Color vertices according to Sperner boundary rules.
- Search for fully-labeled small triangles.
- Randomly generate valid Sperner colorings.
- Count how many trichromatic triangles appear.
- Visualize the path-following proof.

**Questions students can ask:**

- Why must a fully labeled triangle exist?
- Is the number of such triangles always odd?
- What happens if the boundary rule is violated?
- How can this be turned into an algorithm?

**Patterns to discover:**

- Boundary conditions force an interior combinatorial event.
- The number of fully labeled small triangles is odd.
- Sperner's lemma is a discrete fixed-point theorem.

**Mathematical shadows:**

- Sperner's lemma.
- Brouwer fixed point theorem.
- Combinatorial topology.

---

## 16. Fixed-point experiments

**Central question:**  
Can fixed points be found by discrete approximation?

**Experiments:**

- Define maps from a triangle to itself.
- Draw displacement vectors.
- Triangulate the domain.
- Color vertices according to the direction of displacement.
- Use Sperner's lemma to locate approximate fixed points.
- Refine the triangulation and watch the approximation improve.

**Questions students can ask:**

- Why should a map from a disk to itself have a fixed point?
- Can we find fixed points computationally?
- How does the approximation improve under refinement?

**Patterns to discover:**

- Fixed points can be detected combinatorially.
- Sperner's lemma gives an algorithmic shadow of Brouwer.
- Topology can force solutions to equations.

**Mathematical shadows:**

- Brouwer fixed point theorem.
- Sperner approximation.
- Topological existence theorems.

---

## 17. Nim

**Central question:**  
When is a game position winning?

**Experiments:**

- Play Nim.
- Compute winning and losing positions.
- Discover binary xor.
- Simulate random play and optimal play.
- Generalize to subtraction games.
- Compute small Sprague-Grundy values.

**Questions students can ask:**

- Can we classify all winning positions?
- Why does xor appear?
- What changes when the rules change?

**Patterns to discover:**

- Some games have hidden algebraic structure.
- Winning positions can be classified.
- The xor operation appears naturally.

**Mathematical shadows:**

- Impartial combinatorial games.
- Nim-sum.
- Sprague-Grundy theory.

---

## 18. Chomp

**Central question:**  
Can we prove a winning strategy exists without finding it?

**Experiments:**

- Simulate Chomp on small boards.
- Compute winning and losing positions by dynamic programming.
- Visualize the state space.
- Observe first-player winning behavior.
- Try to identify explicit strategies.

**Questions students can ask:**

- Why does the first player win?
- Can we find the winning strategy?
- How can existence be easier than construction?

**Patterns to discover:**

- Strategy stealing can prove existence nonconstructively.
- Explicit strategies can be hard to find.
- Finite games can be solved experimentally for small sizes.

**Mathematical shadows:**

- Strategy stealing.
- Nonconstructive proof.
- Dynamic programming.

---

## 19. Minimax games

**Central question:**  
Can perfect play be computed?

**Experiments:**

- Build tic-tac-toe.
- Construct the game tree.
- Implement minimax.
- Count possible states.
- Compute optimal play.
- Compare:
  - human,
  - random,
  - greedy,
  - minimax agents.
- Visualize the game tree.

**Questions students can ask:**

- Can a game be solved completely?
- Why do game trees grow so quickly?
- What makes a good heuristic?

**Patterns to discover:**

- Some finite games can be solved by backward induction.
- Perfect play can produce draws.
- Game trees grow quickly.

**Mathematical shadows:**

- Minimax.
- Backward induction.
- Search complexity.
- Algorithmic game solving.

---

## 20. Multi-armed bandits

**Central question:**  
How should an agent balance exploration and exploitation?

**Experiments:**

- Simulate slot machines with unknown reward probabilities.
- Try:
  - greedy,
  - epsilon-greedy,
  - UCB,
  - Thompson sampling.
- Track regret.
- Compare strategies.
- Vary uncertainty.

**Questions students can ask:**

- When should one explore?
- When should one exploit?
- How can we measure learning performance?
- Why can a greedy strategy get stuck?

**Patterns to discover:**

- Good decisions require experimentation.
- Exploration has short-term cost but long-term benefit.
- Regret quantifies learning performance.

**Mathematical shadows:**

- Reinforcement learning.
- Regret.
- Bayesian updating.
- Decision-making under uncertainty.

---

## 21. Learning in games

**Central question:**  
Can agents learn to play well?

**Experiments:**

- Implement fictitious play.
- Implement regret matching.
- Use reinforcement learning for simple games.
- Let agents repeatedly update strategies.
- Compare learned strategies with equilibria.
- Study convergence and cycling.

**Questions students can ask:**

- Do agents learn equilibrium strategies?
- When does learning cycle?
- How does exploration affect learning?
- Can simple agents become strong players?

**Patterns to discover:**

- Learning dynamics may converge or cycle.
- Equilibria can emerge from adaptation.
- Some games are hard for learning agents.

**Mathematical shadows:**

- Learning in games.
- Regret minimization.
- Reinforcement learning.
- Adaptive dynamics.

---

## 22. Network games

**Central question:**  
How does the network of interactions affect outcomes?

**Experiments:**

- Place agents on graphs.
- Let them play:
  - coordination games,
  - prisoner's dilemma,
  - public goods games.
- Compare:
  - complete graphs,
  - grids,
  - random graphs,
  - scale-free networks.
- Study diffusion of strategies.
- Visualize clusters.

**Questions students can ask:**

- Do hubs matter?
- Can networks stabilize cooperation?
- How does graph structure change outcomes?

**Patterns to discover:**

- Network topology affects equilibrium and learning.
- Hubs influence outcomes.
- Local interaction can stabilize diversity.

**Mathematical shadows:**

- Network games.
- Graph structure.
- Diffusion of behavior.
