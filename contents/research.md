<strong>Markov chain Monte Carlo</strong>

Markov chain Monte Carlo (MCMC) is the state of art method to sample from a target distribution. One of the most widely used MCMC algorithm is Metropolis-Hastings (MH), which samples from a proposal distribution, and accepts/rejects the newly proposed sample according to the density ratio of the target at the new and current parameter values. The efficiency of the MH algorithm mainly depends on the choice of the proposal distribution.

Our group have developed some new types of MH kernels, including mirror-type kernels and generative-model-assisted kernels. Mirror-type kernels, in contrast to the random walk, generate new candidates around the "mirror image" of the current state to produce negative autocorrelations and super efficiency.

<strong>Phylogenetics</strong>

Phylogenies use trees to describe the evolutionary relationships. Accurate phylogenies provide detailed genealogical maps which show the key transitions during evolution, and phylogenetic reconstruction is the building block for evolutionary biology. 

Phylogenetic inference is typically done using DNA sequence data under the multispecies coalescent (MSC) model. The important parameters in the model are the tree topology, split times and population sizes. Under the Bayesian framework, the updates of split times and population sizes are with-in model MCMC move while the update of the tree topology is between-model move. We use mirror-type kernels plus a new mode of proposal distribution, called driver+passenger to update the within-model parameters, and design a set of between-model moves which incorporate the posterior information of alternate models to improve the efficiency of MCMC. The resulting new algorithms can lead to a factor of 2-10 increase on mixing efficiency in empirical studies. 

