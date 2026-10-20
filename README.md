# Statistical Barrier Certification

**Statistical Certification of Neural Barrier Functions for invariance and Reach-Avoidance in Learning-Enabled Systems**

Zhipeng Cao, Nikolaus Vertovec, Luke Ong, Taoran Wu, Bai Xue

[Read the paper](paper/statistical-barrier-certification.pdf) · [Project website](https://formalcert-ai.github.io/statistical-barrier-certification/) · [FormalCert-AI](https://formalcert-ai.github.io/)

## Overview

This work combines joint controller–barrier learning with independent statistical certification for black-box dynamical systems.

1. Jointly train a policy and neural barrier using PID-Barrier feedback and PPO.
2. Freeze the learned controller and barrier. Collect independent initial states and finite-horizon rollout data.
3. Solve a scalar scenario optimization problem to construct multi-step PAC invariant or reach-avoid regions.

The guarantees quantify the fraction of initial states in a certified region satisfying a finite-horizon property under a fixed reference measure. They are set-level guarantees and do not identify which individual states satisfy the property. Certificate reuse requires the dynamics and controller to remain unchanged.

The paper evaluates an inverted pendulum, a Van der Pol oscillator, and a 10-dimensional Hopfield system, covering invariance and reach-avoidance tasks.

## Release status

The current release contains the **paper PDF**. The research implementation, experiment configuration, and reproduction instructions will be added in subsequent updates. The interactive illustration on the website is an explanatory schematic.

```text
paper/
  statistical-barrier-certification.pdf
README.md
```

Manuscript version: **October 20, 2026**, 26 pages.

## Updating the project

Add the implementation and reproduction instructions to this repository when they are ready. When updating the paper, replace `paper/statistical-barrier-certification.pdf` and the matching website copy at `assets/statistical-barrier-certification.pdf` in [the website repository](https://github.com/FormalCert-AI/formalcert-ai.github.io). Keep the two PDFs byte-identical and update the manuscript date and relevant figures on the project page.

## Citation

```bibtex
@unpublished{cao2026statistical,
  title = {Statistical Certification of Neural Barrier Functions for invariance and Reach-Avoidance in Learning-Enabled Systems},
  author = {Cao, Zhipeng and Vertovec, Nikolaus and Ong, Luke and Wu, Taoran and Xue, Bai},
  year = {2026},
  note = {Preprint},
  url = {https://formalcert-ai.github.io/statistical-barrier-certification/}
}
```
