# Bayesian Neural Networks

## Week 4 & 5 (15 Feb - 28 Feb)

- [Bayesian Deep Learning and a Probabilistic Perspective of Generalization](https://proceedings.neurips.cc/paper/2020/file/322f62469c5e3c7dc3e58f5a4d1ea399-Paper.pdf)
- [How Good is the Bayes Posterior in Deep Neural Networks Really?](https://arxiv.org/abs/2002.02405) (Quite complicated paper with lots of experiments and hypothesises!)
- Training ibnn on Fashion MNIST dataset. At first, training raw images didn't work because the VGG architecture has 5 maxpool2 layers and it needs input of size at least 32x32. So I padded the images. I also reduced the learning rate to make it work. Results so far (accuracy %):

|               | iBNN-VGG16 | VGG16 | BNN-VI-VGG16             |
| ------------- | ---------- | ----- | ------------------------ |
| Fashion MNIST | 92.62      | 92.08 | 10.00 (not well trained) |

|               | iBNN-WideResNet28x10 | WideResNet28x10  |
| ------------- | -------------------- | ---------------- |
| Fashion MNIST | 93.69 (45 epoch)     | 93.65 (90 epoch) |



## Week 3 (8 Feb - 14 Feb)

- [BNN: a tutorial](https://wjmaddox.github.io/assets/BNN_tutorial_CILVR.pdf) from NYU
- [The case for Bayesian Deep Learning](https://cims.nyu.edu/~andrewgw/caseforbdl.pdf) by Andrew Gordon Wilson
- ICML 2020 Tutorial: [Bayesian Deep Learning and Probabilistic Model Construction](https://www.youtube.com/watch?v=E1qhGw8QxqY) by A. G. Wilson

## Week 2 (1 Feb - 7 Feb)

- [NIPS2020 tutorial on Uncertainty Estimation in Deep Learning](https://slideslive.com/38935801/practical-uncertainty-estimation-outofdistribution-robustness-in-deep-learning)

## Week 1 (24 Jan - 31 Jan)

### Objectives

- [ ] Read and underestand the paper [Scalable Bayesian neural networks by layer-wise input augmentation](https://arxiv.org/abs/2010.13498) (iBNN)
  - I underestood the main idea of the paper (the section "Layer-wise input priors"). However, I need more time to undrestand the details (the sections "Variational inference", "Variational ensemble posterior", "Uncertainty decomposition").
- [ ] Implement iBNN and test it on FashionMNIST.
  - I cloned the ibnn repo and trained VGG on Cifar10.

### What I've learned or done
- Veriational inference:
  - [Princeton lecture note](https://www.cs.princeton.edu/courses/archive/fall11/cos597C/lectures/variational-inference-i.pdf)
- [Bayesian Mixture Models and the Gibbs Sampler](http://www.cs.columbia.edu/~blei/fogm/2015F/notes/mixtures-and-gibbs.pdf)
- [An article on Stochastic Weight Averaging (SWA)](https://pytorch.org/blog/pytorch-1.6-now-includes-stochastic-weight-averaging/)
