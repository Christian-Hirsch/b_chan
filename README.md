# Maximum likelihood calibration of stochastic multipath radio channel models

When a signal is sent from one location to another, the receiver typically obtains a distorted version of the original message. Indeed, besides traveling along the direct connection path, the signal is subject to a large number of reflections and refractions, so that the final signal becomes a random superposition over the different transmission paths. How precisely the superpositions are created is the subject of stochastic channel models. Since channel modeling lies at the very foundation of wireless communication, poor modeling at this layer can severely distort the interpretation and validity of simulation results for more complex communication systems. But how to find a suitable model with reasonable parameters? How to determine if one model is better than another.

<p align="center">
<img src="https://christian-hirsch.netlify.app/project/channel/featured_hu2257b063ef9c7e6a4f773bcb84099a30_111912_720x0_resize_lanczos_2.png" /></a>
</p>

In a [paper](https://vbn.aau.dk/en/publications/maximum-likelihood-calibration-of-stochastic-multipath-radio-chan-2) with [A. Bharti](https://vbn.aau.dk/en/persons/141882), [T. Pedersen](https://vbn.aau.dk/en/persons/106895) and [R. Waagepetersen](https://people.math.aau.dk/~rw/), we highlight the features and challenges to approach this topic through maximum likelihood estimation. The channel model is typically set in the time domain, whereas the measurement dictates that observations come from the frequency domain. Therefore, the estimation problem becomes an instance of a latent-variable model, and we rely on MCMC-techniques from Bayesian statistics to approach this multi-faceted issue. In particular, we elucidate how to leverage parallel tempering to overcome the challenge of slow mixing.

The present [notebook](inhomogeneous.ipynb) contains a worked-out example in R of how to apply the methodology to simulated and real datasets.
