# ResearchPapers
World Models:
1) World Models - David Ha 1 Jurgen Schmidhuber (2018) https://arxiv.org/pdf/1803.10122
   <img width="375" height="229" alt="{7814E704-5C9E-4D31-839A-2D1D79CF7EF5}" src="https://github.com/user-attachments/assets/ed2580cd-09f0-4ad7-8720-f7b186b11ceb" />
   The agent’s architecture is divided into three distinct modules:
   * V (Vision): a Variational Autoencoder (VAE) that compresses high-dimensional observations (images) into a lower-dimensional latent vector zₜ. This captures the essential spatial features of each frame.
   * M (Memory): a Mixture-Density Network Recurrent Neural Network (MDN-RNN) that models the temporal dynamics—in other words, it predicts what the next latent vector will be given the current latent state, the action taken, and its internal memory (hₜ). It outputs parameters for a mixture of Gaussians, allowing stochastic sampling of the next latent vector zₜ₊₁.
   * C (Controller): a lightweight linear model that takes as input the current latent vector zₜ and the hidden state hₜ, and outputs an action aₜ. This module is trained not via backpropagation, but using an evolutionary strategy (CMA-ES), keeping the controller compact and tractable.

3) 
