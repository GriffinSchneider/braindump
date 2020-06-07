+++
title = "Meta Learning"
author = ["Jethro Kuan"]
lastmod = 2020-05-31T20:20:15+08:00
draft = false
+++

### Backlinks {#backlinks}

- [Differentiable plasticity: training plastic neural networks with backpropagation]({{< relref "miconi_differentiable_plasticity" >}})
- [A critique of pure learning and what artificial neural networks can learn from animal brains]({{< relref "zador19_critique_pure_learning" >}})

tags
: [Reinforcement Learning ⭐]({{< relref "reinforcement_learning" >}})

Learning to learn: learn an update rule from related tasks

For example, tasks are related through a low-dimensional embedding.

{{< figure src="/ox-hugo/screenshot2019-12-11_17-03-01_.png" >}}

## Model-Agnostic Meta Learning (MAML) {#model-agnostic-meta-learning--maml}

Based on 2nd-order gradient descent:

2-stage gradient-based approach on batches of tasks \\(\mathcal{T}\\):

1.  Inner loop:

\begin{equation}
\theta_i' = \theta - \alpha \nabla\_\theta L\_{\mathcal{T}}(f\_\theta)
\end{equation}

1.  Outer Loop:

\begin{equation}
\theta=\theta-\beta \nabla\_{\theta} \sum\_{\mathcal{T}\_{i} \sim p(\mathcal{T})} \mathcal{L}\_{\mathcal{J}\_{i}}\left(f\_{\theta\_{i}^{\prime}}\right)
\end{equation}

## Resources {#resources}

- [ICML 2019 Meta-learning Tutorial](https://sites.google.com/view/icml19metalearning)

### Backlinks {#backlinks}

- [Differentiable plasticity: training plastic neural networks with backpropagation]({{< relref "miconi_differentiable_plasticity" >}})
- [A critique of pure learning and what artificial neural networks can learn from animal brains]({{< relref "zador19_critique_pure_learning" >}})