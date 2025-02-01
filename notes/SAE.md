# sparse auto encoders

- get their input from the activation layer
- autoencoder maps (encodes) existing `n` dimensions to `m` dimensions (where `m` > `n`)
    - this is because due to superposition, a neuron can activate on multiple features.
    - to extract multiple features from a few neurons, the activation function output is mapped on to higher dimensions to extract all the features.
- the autoencoder then decodes these features back into `n` dimensions 
    - the higher dimension vector is then projected back into the lower dimensions but with features being geometrically orthogonal to each other