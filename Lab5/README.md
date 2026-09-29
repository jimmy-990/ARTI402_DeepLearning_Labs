# Lab 5 

- Training loop: forward -> loss -> backward (gradients) -> optimizer step -> repeat
- Backprop: chain rule in reverse (loss -> dense2 -> ReLU -> dense1)
- Epoch = full pass over the data; iteration = one weight update
- Mini-batches = more updates per epoch (32 is good, 8 is too noisy)

| Optimizer | Idea | Fixes |
|---|---|---|
| SGD | w -= lr * grad | baseline |
| Momentum | remembers direction | zig-zag |
| RMSProp | per-parameter step by gradient size | one step size for all |
| Adam | momentum + RMSProp + correction | combines both |

- Adam correction uses t = iterations + 1 (else division by zero)
- Adam still needs a good learning rate
- Best result: 0.96 train vs 0.82 test (overfitting)
