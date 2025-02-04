# sparse auto encoders

- get their input from the activation layer
- autoencoder maps (encodes) existing `n` dimensions to `m` dimensions (where `m` > `n`)
    - this is because due to superposition, a neuron can activate on multiple features.
    - to extract multiple features from a few neurons, the activation function output is mapped on to higher dimensions to extract all the features.
- the autoencoder then decodes these features back into `n` dimensions 
    - the higher dimension vector is then projected back into the lower dimensions but with features being geometrically orthogonal to each other


```text
It's important not to get confused between the autoencoder and model's notation. Remember - the model takes in features  x , maps them to lower-dimensional vectors  h , and then reconstructs them as  x′ . The autoencoder takes in these hidden states  h , maps them to a higher-dimensional but sparse vector  z , and then reconstructs them as  h′ . Our hope is that the elements of  z  correspond to the features of  x .
```
[^ verbatim from this colab notebook](https://colab.research.google.com/github/callummcdougall/ARENA_3.0/blob/main/chapter1_transformer_interp/exercises/part31_superposition_and_saes/1.3.1_Toy_Models_of_Superposition_&_SAEs_solutions.ipynb?t=20250127#scrollTo=SYxwPHHTs4Pl)