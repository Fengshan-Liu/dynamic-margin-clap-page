# Dynamic Margin CLAP: Adaptive Positive-Pair Margins for Audio-Text Retrieval

**ACM Multimedia 2026** · [Project page](https://fengshan-liu.github.io/dynamic-margin-clap-page/) · [Paper (PDF)](https://fengshan-liu.github.io/dynamic-margin-clap-page/assets/dynamic-margin-clap-paper.pdf)

Dynamic Margin CLAP studies how caption specificity can guide audio–text contrastive learning. It assigns each matched audio–caption pair a training-time positive-pair margin based on the normalised inverse document frequency of the caption tokens. More specific descriptions receive a stronger alignment requirement. The margin is removed at inference.

The method is evaluated with Euclidean and two Lorentz-hyperbolic embeddings on WavCaps–FreeSound, Clotho, and MACS. The dynamic margin improves mean recall in all nine corpus–geometry comparisons against the corresponding no-margin baselines. The additional benefit of hyperbolic geometry depends on the corpus.

## Authors

Haoran Liang¹², Fengshan Liu¹, Selene Zhu³, Yueling Yang¹, and Xuanting Li⁴

- ¹ Xi’an Jiaotong-Liverpool University, AIAC
- ² INSAIT
- ³ Ruijie Networks
- ⁴ Xi’an Jiaotong-Liverpool University, SAT

## Results at a glance

Change in mean recall (ΔMR) from adding the dynamic margin, averaged over five seeds:

| Corpus | Euclidean | DirectLift | ExpMap |
| --- | ---: | ---: | ---: |
| WavCaps–FreeSound | +0.002683 | +0.005271 | +0.004943 |
| Clotho | +0.005422 | +0.005837 | +0.004874 |
| MACS | +0.001429 | +0.001816 | +0.001668 |

These values compare each margin variant with its matching no-margin control. They do not establish a uniform advantage for hyperbolic geometry across corpora.

## Materials

| Resource | Status |
| --- | --- |
| [Paper](https://fengshan-liu.github.io/dynamic-margin-clap-page/assets/dynamic-margin-clap-paper.pdf) | Available |
| Supplementary material | Coming soon |
| Poster | Coming soon |

## About this repository

This repository contains the static project website and the paper PDF. It does not contain training, evaluation, or model source code. The site is published with GitHub Pages from the `main` branch at the repository root.

For conference information, see [ACM Multimedia 2026](https://2026.acmmm.org/).
