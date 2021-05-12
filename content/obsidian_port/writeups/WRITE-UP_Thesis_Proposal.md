+++
 author = "Anonymous"
 title = "WRITE-UP Thesis Proposal"
 date = 2021-05-12
+++




# Introduction
Generally speaking, success in work is determined by general intelligence and conscientiousness [1]. We can think of conscientiousness $C: \Pi \to \mathbb{R}$ as a factor characterizing the distribution over success which an agent can expect, given his emotional policy $\pi \in \Pi$ which takes an agent's history and generates a behavior; for simplicity's sake, we can for the sake of argument associate $C\_g(\pi)$ with the median of the success distribution induced by $\pi$, for an agent with fixed intelligence $g$.

While there is a genetic component to $C$ (apparently anti-correlated [2] with $g$, as one would expect given [Berkson's Law](https://www.processingstochasticites.com/obsidian_port/writeups/Berksons_Law/)), there is a significant environmental factor (around 50% [3]). Furthermore, conscientiousness changes over an individual's lifetime, often for the better [4].

Oftentimes, failures of conscientiousness (procrastination, irresponsibility, etc) are chalked up to biases of human cognition such as hyperbolic discounting. However, this pessimistic view may not adequately explain the wide variation observed, nor the fact that conscientiousness does change over long time horizons. 

Naively, one would expect genes conferring high conscientiousness to reach fixation in a population very rapidly; unlike intelligence, which we would a priori expect to remain normally distributed as there are structural reasons suggesting that upward mean drift would be slow and selection for levels above the mammalian average was first applied somewhat recently in our evolutionary history, conscientiousness should have a nearer asymptotic fitness bound (presumably modifying a discount rate is easier to do than modifying $g$) and should have been selected for over a long time horizon (high intelligence is circumstantially useful; a good emotional policy is always useful). 

Moreover, the naive observer should be highly surprised that conscientiousness changes positively over one's lifespan, but slowly so. Is the emotional brain always such a slow learner?

I seek to use evolutionary game theory to demonstate a plausible mechanism by which these surprising facts (high genetic variation in $C(\pi)$, high environmental variation in $C(\pi)$, and submartingale-like behavior of $C(\pi)$) may be rationalized.

# Formalism

## Model
We represent the community of agents by $\mathcal{A}$ and a discrete status function $s: \mathcal{A} \to [0,1]$ for which $\sum\_{A\in \mathcal{A}} s(A) = 1$.

We assume that one's emotional policy can only be lossily inferred by others; specifically, one's current "real" conscientiousness ($C\_t$) is noisily encoded by others as $C\_t'$ according to the function $C\_t' = C\_{t-s} + \epsilon, \epsilon \sim N(0,\sigma\_C)$, where $s$ is some delay factor. 

We assume that general intelligence in the population is distributed according to $g \sim N(\mu\_g,\sigma\_g)$ and is fixed over a lifetime.

We assume that each agent $A \in \mathcal{A}$ generates resources $r^A\_t$ the following production function: $r^A\_t = \alpha g^{\beta} C\_t^{1-\beta}$, where $\alpha,\beta \in (0,1)$ and $\alpha$ is a one-off self-imposed handicap.

In each period, an agent can devote resources to up to two things: 

(1) Investing:

The agent has long-term wealth $w$ which is a store of resources, and can invest up to $r^A\_t - B/n$ in a given time period (the rest is used communally).

(2) Challenging the current hierarchy:

The agent can attempt to induce a new status function $s'$, whereupon he succeeds with probability $p = w\delta/\sum\_{A} |s'(A)-s(A)|^2$ (where $\delta$ is an appropriate scale factor) and dies otherwise.

He also chooses the handicap $\alpha$ every period.

Each period, if $\sum\_{A \in \mathcal{A}} r^A\_t < B$, each agent dies with probability $1-\sum\_{A \in \mathcal{A}} r^A\_t/B$.

Each agent lives for $T$ periods unless killed. Whenever an agent dies, a new agent is created whose emotional policy $\pi$ is given by a RV using $s$ as a density on $\{\pi\_A, A \in \mathcal{A}\}$. 

We say that an agent can have an executive strategy $\rho$ over his per-period choice of $\alpha$ and his choice to induce a new status function.
# Theorems
## Theorem 2: Hierarchy is an ESS
Punchline: show that a status well-ordering on the set of agents is stable due to fight rules (which themselves are microfounded in resource abundance)
## Theorem 2.1: Conscientiousness pays differentially in a hierarchy
Punchline: having maximally high conscientiousness is crucial at the top of the hierarchy. high conscientiousness anywhere else gets you designated as a threat.
## Theorem 2.2: Slowly Increasing Conscientiousness pays in a hierarchy
Punchline: as one grows older, one expects to rise up in the hierarchy due to churn and deaths. So, slowly increasing conscientiousness is useful.
## Theorem 3: Egalitarianism is an ESS
Punchline: show that egalitarianism is stable because of first-mover disadvantage
## Theorem 3.1: Moderate Conscientiousness pays in an egalitarian society
Punchline: too high conscientiousness will get one killed for mooching. too high will get one killed for being a threat.
## Theorem 3.2 Slowly Increasing Conscientiousness pays in an egalitarian society
Punchline: as one grows older, one accumulates more wealth and thus becomes more greatly able to prevent/correct uprisings. Therefore, one can collect rents by increasing his status moderately with age. So, slowly increasing conscientiousness is useful.

References 

(1) (https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1744-6570.1999.tb00174.x)
(2) (https://www.sciencedirect.com/science/article/abs/pii/S1041608005000348?via%3Dihub)
(3) https://pubmed.ncbi.nlm.nih.gov/27337136/
(4) https://www.apa.org/monitor/julaug03/personality
 
 <iframe seamless src="/obsidian_port/writeups/nodes/WRITE-UP_Thesis_Proposal.html" style="width:700px; height:400px; border: 2px solid black"></iframe>