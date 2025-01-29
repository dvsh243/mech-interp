# need to know transformers modules
- LayerNorm (transforming the input to have zero mean and unit variance)
- Positional embedding (a lookup table from position indices to residual stream vectors)
- Attention (the method of computing attention patterns for residual stream vectors)
- MLP (the collection of linear and nonlinear transformations which operate on each residual stream vector in the same way)
- Embedding (a lookup table from tokens to residual stream vectors)
- Unembedding (a matrix for converting residual stream vectors into a distribution over tokens)


## logits
- given an arbitrary vector `x`, we can turn it into a probability distribution via the `softmax` function.

## imp terms
- ### BPE (byte pair encodings)
- ### attention as a generalized convolution
- ### learned and absolute positional embeddings