<!-- Profile README for github.com/jakomycat — search for "TODO" before publishing. -->

<p align="center">
  <img src="./assets/header.svg" width="100%" alt="Jacobo Chalarca Vásquez — Scientific Machine Learning: PINNs, neural operators, numerical PDEs. Animated tracer particles flowing through a von Kármán vortex street.">
</p>

<p align="center">
  I build neural PDE solvers, <b>physics-informed neural networks</b> and <b>neural operators</b>, and study when they work and where they break.
</p>

<img src="./assets/divider.svg" width="100%" alt="">

### About

- **Studying:** B.Sc. Computer Science, Universidad Nacional de Colombia, Manizales (graduating 2027)
- **Main focus:** Scientific ML, including PINNs, neural operators (FNO, DeepONet) and numerical PDEs
- **Also:** interpretability of language models
- **Teaching:** teaching assistant for *Intro to Computer Science* and *Machine Learning* (2024-2 to 2026-1)
- **Open to:** research internships in SciML / scientific computing, summer 2027 <!-- TODO: adjust or remove -->
- **Contact:** <!-- TODO: institutional email · ORCID · Google Scholar · CV -->

<img src="./assets/divider.svg" width="100%" alt="">

### Projects

Each project has a tier: my own ranking of how well it represents my work, from S (flagship) down.

<p>
  <img src="./assets/tier-s.svg" height="22" alt="Tier S">&nbsp;
  <img src="./assets/tier-a.svg" height="22" alt="Tier A">&nbsp;
  <img src="./assets/tier-b.svg" height="22" alt="Tier B">&nbsp;
  <img src="./assets/tier-c.svg" height="22" alt="Tier C">&nbsp;
  <img src="./assets/tier-d.svg" height="22" alt="Tier D">
</p>

<img src="./assets/divider.svg" width="100%" alt="">

### Scientific ML projects

#### <img src="./assets/tier-s.svg" height="22" alt="Tier S"> &nbsp;Padding and boundary conditions in Fourier Neural Operators &nbsp;`in progress`

Fourier Neural Operators compute their spectral convolutions with the FFT, which assumes the domain is periodic. Non-periodic problems are usually handled by padding the input, but the choice of padding is rarely examined. This project compares zero, reflect, replicate and Fourier-continuation padding, at several padding lengths, under periodic, Dirichlet, Neumann and absorbing boundary conditions. Every setting uses the same FNO and several random seeds. The goal is a practical guide to which padding to use, and how much of it, for each type of boundary.

*Work in progress: no code or results are public yet.*

<img src="./assets/divider.svg" width="100%" alt="">

### Interpretability projects

#### <img src="./assets/tier-a.svg" height="22" alt="Tier A"> &nbsp;Does BETO learn like BERT?

This project reproduces four classic analyses of what BERT encodes at each layer (Jawahar et al., 2019) and extends them to Spanish with BETO. The four analyses are phrase chunking, nine probing tasks, subject–verb agreement, and compositional structure with tensor product decomposition networks. Every experiment runs over five seeds. Randomly initialised encoders serve as a control, separating what pretraining adds from what the architecture already provides. Comparisons use paired t-tests with Benjamini–Hochberg correction.

**Repository →** [jakomycat/does-beto-learn-like-bert](https://github.com/jakomycat/does-beto-learn-like-bert)

#### <img src="./assets/tier-c.svg" height="22" alt="Tier C"> &nbsp;Logit Lens vs. Tuned Lens

This project compares two ways of reading the intermediate layers of GPT-2 Small. The logit lens decodes every hidden state with the model's final unembedding. The tuned lens first learns an affine map for each layer. The two are compared on KL divergence to the final output, mean reciprocal rank, cumulative hit rate, and the first layer that predicts correctly, broken down by prompt type: knowledge, arithmetic, sequences and syntax.

**Repository →** [jakomycat/logit-lens-vs-tuned-lens](https://github.com/jakomycat/logit-lens-vs-tuned-lens)

<img src="./assets/divider.svg" width="100%" alt="">

### Toolbox

`Python` `PyTorch` `NumPy` `Hugging Face Transformers` `Jupyter` `LaTeX` `Git`
<!-- TODO: add/remove to match what you actually use -->

<p align="right"><sub>Header: tracer particles advected through a von Kármán vortex street (point-vortex model, co-moving frame, RK4).</sub></p>
