+++
 author = "Anonymous"
 title = "Endogenous Risk Attitudes"
 date = 2021-05-11
+++

label:writeups
SAFE2PUBLISH

Scale in the Fly's Eye
Does Encoding Affect Behavior?
Netzer '09, Robson '01

For stochastic measurement, we can either guess that input is stochastic and measurement true, or input constant and measurement error-prone. Finds $E[m^-1(x)]$ vs $m^-1(E(x))$
$m$ increasing and therefore invertible

[Psychophysics](https://www.processingstochasticites.com/obsidian_port/writeups/Psychophysics/) rationale for s-shaped utility, encoding of stimuli.

Khaw&Li&Woodford '20, Frydman&Jin '19

Optimal perception of lotteries (over-sampling of low-prob), surprising risk (perception-driven risk attitudes)

Decision problem: lottery vs safe option (observation of probabilities and s, friction over vector of rewards)

Encoding function, sampling frequencies. Encoding function is noisy, use MLE/Bayesian over encoded data to guess true vector. Look at nearly complete information ($n \to \infty$), whereupon Bayesian/MLE equate.

Ex Ante Optimization
$\min L(n) = \mathbb{E}[\max\{r,s\} - 1_{q_n>s}r - 1_{q_n \leq s}s$

Theorem (Limit Loss)
Under a regularity condition, loss grows like 1/n and which acts as expectation over MSE conditional on tie (condition because perception errors small) (MSE because distortion only occurs if s occurs between r and $q_n$, prob of choice distortion and loss both related to error, so total loss related to square of error)

[Dominated Convergence](https://www.processingstochasticites.com/obsidian_port/writeups/Dominated_Convergence/)

allocation problem: must focus area of neighborhood of $r$ and must focus over arms.
$m$ is bounded, so steepness (and area focus ) is limited.

Optimal encoding function is s-shaped (convex-below,concave-above modal reward)

Over-sampling of low-prob arms (s-shape makes info from tails sparser)

Mispecification can be cast as EU with bernoulli (or other) transform. May be explained by need to avoid complex procedures.

White '82

Asympototic MLE minimizes KL-divergence

Omitted variable — lack of information can induce apparent risk attitudes.

Prior on low risk compresses perceived divergence in lottery and pushes to the left for bournelli encoding function.

Perception errors can persist despite copious information due to misspecified learning. 

Adaptation channels: optimal encoding and/or anticipation of lotteries.
 
 <iframe seamless src="/obsidian_port/writeups/nodes/Endogenous_Risk_Attitudes.html" style="width:700px; height:400px; border: 2px solid black"></iframe>