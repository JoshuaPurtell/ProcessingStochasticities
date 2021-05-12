+++
 author = "Anonymous"
 title = "Selection Problems In The Presence Of Implicit Biases"
 date = 2021-05-12
+++

label:writeups
SAFE2PUBLISH

Micro Theory Talk given by Nisheeth Vishnoi, Yale University

Problem: selection decisions in social contexts (job, academic, etc)

Subset selection problem: select $n$ individuals with highest total utility.

Model of implicit bias: apply $\beta \in [0,1]$ multiplicatively to latent utility in order to get observed utility.

Goal: design mechanism to minimize impact of implicit bias.

Generalized Rooney rule: require at least $l \geq 1$ candidates from group to be interviewed.

Long-term impact of Rooney rule.

Dynamic system: 
evidence against implicit bias $a^t>1$, $a^{(t+1)}:=a^t\frac{u\_{latent}}{u\_{observed}}$
implicit bias is rv sampled from distribution

Punchline is that implicit bias rapidly decays with Rooney rule.

Any non-intersectional intervention can only guarantee only fraction of the utility achievable absent bias (~8/9)
 
 <iframe seamless src="/obsidian_port/writeups/nodes/Selection_Problems_In_The_Presence_Of_Implicit_Biases.html" style="width:700px; height:400px; border: 2px solid black"></iframe>