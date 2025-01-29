# attention
- casual attention
- bidirectional attention

## the difference
Comparison with Bidirectional Models (e.g., BERT)
- GPT (Causal Transformer) -> Uses causal masking for left-to-right generation.
- BERT (Bidirectional Transformer) -> Sees both past and future tokens (no causal mask), so it’s used for tasks like classification and filling missing words.


## why not use future tokens for casual attention?
If the model could access future tokens:

During training: It would learn to rely on words that haven’t been generated yet, making it useless for actual text generation.
During inference: It wouldn’t work at all, because the next token does not exist until it's generated.

