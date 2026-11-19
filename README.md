<p align="center">
  <img src="asset/avatar/raa-logo.png" width="200" alt="Resolution as Attention logo, an ink-wash plum blossom branch">
</p>

<h1 align="center">Resolution as Attention for Efficient Agent Memory Perception</h1>

<p align="center">
  <a href="https://arxiv.org/abs/2611.24422"><img src="https://img.shields.io/badge/arXiv-2611.24422-b31b1b.svg" alt="arXiv"></a>
  <a href="https://sxiangag.github.io/resolution-as-attention/"><img src="https://img.shields.io/badge/Project-Page-2F6B5B.svg" alt="Project Page"></a>
</p>

This is the official repository for the paper *Resolution as Attention for Efficient Agent Memory Perception*.

## 🔎 Overview

Resolution as Attention (RAA) is a memory perception mechanism that uses visual resolution as a means of attention allocation across interaction histories. RAA renders past interactions as images and dynamically adjusts their resolution at every step according to their relevance to the agent's upcoming decision, preserving fine-grained information for critical interactions while reducing visual-token consumption for less relevant ones.

<p align="center">
  <a href="docs/assets/overview.png"><img src="docs/assets/overview.png" width="900" alt="Overview of Resolution as Attention"></a>
</p>

## ✨ Key Features

- **Relevance estimation**: a 0.6B estimator, fine-tuned from Qwen3-Reranker, scores every past interaction against the task and the latest step.
- **Resolution-controlled rendering**: a learnable sigmoid maps each score to a scale, and each interaction is rendered once as a canonical image and resized to that scale before the agent perceives it.
- **Plug-in perception layer**: RAA transfers to off-the-shelf vision-capable agents and composes with existing memory management methods.

## 🚀 Code

The full code will be released upon the acceptance of the paper.

## 📝 Citation

```bibtex
@article{xiang2026resolution,
  title   = {Resolution as Attention for Efficient Agent Memory Perception},
  author  = {Xiang, Siqi and Xu, Zhipeng and Liu, Shengrui and Chen, Zulong and Miao, Chunyan and Lu, Shijian},
  journal = {arXiv preprint arXiv:2611.24422},
  year    = {2026},
  url     = {https://arxiv.org/abs/2611.24422}
}
```
