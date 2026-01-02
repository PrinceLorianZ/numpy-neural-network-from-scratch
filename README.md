# NumPy Neural Network From Scratch

A fully-connected neural network implemented from scratch using **NumPy**, focusing on understanding and debugging **forward propagation + backpropagation** (no deep learning frameworks).  
Repo: https://github.com/PrinceLorianZ/numpy-neural-network-from-scratch.git

## What’s inside
- Configurable MLP architecture (ReLU hidden layers + Sigmoid output)
- Manual implementation of:
  - Parameter initialization (W, b)
  - Forward propagation (Linear → Activation)
  - Binary cross-entropy loss
  - Backpropagation (dA, dZ, dW, db)
  - Gradient descent updates
- Simple training loop with loss/accuracy tracking
- Demo on a 2D binary classification dataset (e.g., `make_moons`)

## Why I built this
Most ML libraries hide gradient computation. I built this project to truly understand:
- how gradients flow through multiple layers (chain rule)
- why training becomes unstable when shapes/derivatives are wrong
- how to make training reproducible and debuggable (cache `A`/`Z`, sanity checks)

