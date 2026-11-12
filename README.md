<div align="center">

# Raina Liu

**Quantum reliability · Verification · Reproducible scientific software**

I build reproducible experiments that reveal what conventional success metrics fail to measure.

[![Featured: Q-Reliability Lab](https://img.shields.io/badge/Featured-Q--Reliability_Lab-24292f?style=for-the-badge&logo=github)](https://github.com/Raina-ya/q-reliability-lab)
[![Interactive lab](https://img.shields.io/badge/Interactive-Lab-2ea44f?style=for-the-badge)](https://raina-ya.github.io/q-reliability-lab/)
[![Paper](https://img.shields.io/badge/Paper-PDF-b31b1b?style=for-the-badge)](https://github.com/Raina-ya/q-reliability-lab/blob/main/paper/main.pdf)
[![Slides](https://img.shields.io/badge/Slides-PDF-0969da?style=for-the-badge)](https://github.com/Raina-ya/q-reliability-lab/blob/main/slides/q-reliability-lab.pdf)

</div>

---

## Research focus

My work examines **reliability, verification, and benchmarking in noisy quantum computation**: cases where a system looks successful under one metric while its underlying state has already degraded.

I combine analytic derivation, density-matrix simulation, regression tests, and interactive visualization so that every claim can be checked end to end.

## Featured research: Q-Reliability Lab

> **Can a Bell-state circuit receive a perfect score after a phase error has changed the state?**

A phase-flip channel with probability $p$ is applied to one qubit of the Bell state $|\Phi^+\rangle$. The standard computational-basis check never notices:

| Metric | Value under phase flip | What it detects |
| :--- | :---: | :--- |
| Z-basis success $S(p)$ | $1$ | Nothing. The score stays perfect. |
| X-basis correlated success $S_X(p)$ | $1-p$ | The phase error |
| Bell-state fidelity $F(p)$ | $1-p$ | Loss of the target state |

<p align="center">
  <a href="https://github.com/Raina-ya/q-reliability-lab">
    <img src="https://raw.githubusercontent.com/Raina-ya/q-reliability-lab/main/paper/figures/success_vs_fidelity.png" width="720" alt="Computational-basis success remains perfect while Bell-state fidelity decreases.">
  </a>
</p>

**What the repository includes**

- A 101-point density-matrix sweep, checked against closed-form analytic results
- A pre-registered 3,000-row finite-shot sweep with Wilson confidence intervals
- A three-channel × five-metric sensitivity comparison
- Analytic, physical-invariant, and regression tests running in CI
- A dependency-free interactive lab, verified against the Python model

[Interactive lab](https://raina-ya.github.io/q-reliability-lab/) · [Full paper](https://github.com/Raina-ya/q-reliability-lab/blob/main/paper/main.pdf) · [Presentation](https://github.com/Raina-ya/q-reliability-lab/blob/main/slides/q-reliability-lab.pdf) · [Source and data](https://github.com/Raina-ya/q-reliability-lab)

## Other projects

| Project | Question |
| :--- | :--- |
| [bias-probe-visibility](https://github.com/Raina-ya/bias-probe-visibility) | When can runtime probes detect decision-flipping bias in noisy quantum computation, and when can't they? |
| [adaptive-qem-benchmark](https://github.com/Raina-ya/adaptive-qem-benchmark) | How do unmitigated, readout-mitigated, and linear zero-noise-extrapolation results compare under a controlled simulator benchmark? |

## Current direction

- Quantum reliability and metric blind spots
- Error-mitigation benchmarking
- Reproducible scientific software
- Interactive explanations of counterintuitive physical results

## Toolkit

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat-square)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

## Research standards

- **Hypotheses first:** research questions and expected outcomes are recorded before a sweep is run.
- **Fully regenerable:** every figure and table can be rebuilt from the source code and its tests.
- **Honest labeling:** published results come from classical simulation unless explicitly labeled otherwise. I do not present simulated or fake-backend output as quantum-hardware evidence.
