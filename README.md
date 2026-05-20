# Arindam Roy, Ph.D. | Researcher

**Palaeobiology | Artificial Intelligence | Functional Morphology | Biomechanics | Taphonomy | Biogeochemistry**

I am a palaeobiologist and computational researcher working at the intersection of deep learning, experimental taphonomy, and vertebrate palaeontology. My research asks how biological information — colour, morphology, chemistry — survives the fossilisation process, and how modern AI can be used to extract that information at scale. Currently a Marie Skłodowska-Curie Actions Postdoctoral Fellow at the University of Birmingham, I develop self-supervised deep learning pipelines for automated CT segmentation of fossil specimens, with the broader goal of breaking the manual bottleneck that constrains large-scale morphological data collection in palaeontology.

---

## Research Interests

I work on two interconnected problems. The first is taphonomic: what happens to biological pigments — melanins, carotenoids, psittacofulvins — during diagenesis, and how can we distinguish genuine fossil colour signals from artefacts of preservation? I address this through experimental maturation, multi-spectroscopic analysis (ToF-SIMS, FT-IR, Raman, UV-Vis), and laser-stimulated fluorescence imaging. The second is methodological: how can self-supervised and contrastive deep learning reduce the expert-time bottleneck in fossil CT segmentation, enabling morphological analyses at a scale previously impossible? Together these questions feed into a broader interest in the evolutionary biology of Mesozoic vertebrates — dinosaurs, early birds, and their relatives — and how quantitative, reproducible methods can resolve long-standing debates about their ecology, flight origins, and integumentary evolution.

---

## Technical Expertise

| Category | Skills & Tools |
| --- | --- |
| **Languages** | Python, R, JMP, MATLAB/Octave, Bash |
| **Machine Learning & AI** | PyTorch, TensorFlow, SimCLR, MoCo v2, U-Net, ResNet, VAE, Scikit-learn |
| **Imaging & Spectroscopy** | CT segmentation (Avizo, Meshlab, Blender), UV/Laser-Stimulated Fluorescence, ToF-SIMS, FT-IR, Raman, SEM/EDX, 3D Photogrammetry |
| **Bioinformatics & Statistics** | Macroevolutionary modelling, Geometric Morphometrics, Decay/Maturation Experiments |
| **Infrastructure** | GitHub Actions CI/CD, Docker, HPC (BlueBEAR, SLURM), GNU GPL open-source workflows |
| **Visualisation** | ggplot2, Python (matplotlib/seaborn), R, Blender |

---

## Public Repositories & Open-Source Software

---

### Deep Learning for Fossil CT Segmentation (DEEPCTSEG)

- **[DEEPCTSEG v1.0.0 — SimCLR-v1 + U-Net](https://github.com/roy-arindam-1991/Simclr-v1-50k-automated-pipeline)**: Can self-supervised contrastive learning reduce the expert-annotation bottleneck in fossil CT segmentation? End-to-end automated pipeline implementing SimCLR v1 (Chen et al., 2020) — stochastic data augmentation, a shared ResNet encoder, MLP projection head, and NT-Xent contrastive loss — followed by U-Net segmentation with deterministic masking, trained on 50,000 fossil CT images. Provides a reproducible benchmark for label-efficient fossil segmentation at scale. (DOI: [10.5281/zenodo.20242346](https://doi.org/10.5281/zenodo.20242346). GNU GPL v3.0.)

- **[DEEPCTSEG v1.1.0 — MoCo-v2 + U-Net](https://github.com/roy-arindam-1991/MoCo-v2-50k-automated-pipeline)**: Does Momentum Contrast outperform SimCLR when memory efficiency and large negative-sample queues matter? Automated pipeline implementing MoCo v2 (Chen et al., 2020) — a momentum encoder updated via exponential moving average, a dynamic negative-sample queue of up to 65,536 keys, and an MLP projection head — trained on 50,000 fossil CT images under matched data conditions to v1.0.0. Designed for direct controlled comparison of contrastive learning strategies. (DOI: [10.5281/zenodo.20255058](https://doi.org/10.5281/zenodo.20255058).)

*Both pipelines underpin the preprint: Roy et al. (2026) "Breaking the Bottleneck: Fully-automated CT Segmentation of Fossils using Self-Supervised Deep Learning." Submitted to Nature Machine Intelligence.*

---

### Machine Learning for Palaeocolour Reconstruction

- **[SimCLR-v1-50k-automated-pipeline](https://github.com/roy-arindam-1991/Simclr-v1-50k-automated-pipeline)**: Representation learning framework for morphological classification tasks in fossil material. Automated training, checkpointing, and linear evaluation pipeline enabling reproducible benchmarking of label-efficient visual learning on palaeontological image data.

- **[MoCo-v2-50k-automated-pipeline](https://github.com/roy-arindam-1991/MoCo-v2-50k-automated-pipeline)**: Memory-efficient contrastive learning pipeline enabling large-batch-equivalent training without proportional GPU memory scaling — critical for high-resolution fossil CT image datasets where batch size is hardware-constrained.

---

## Selected Publications

### Journal Articles

- **Roy, A.**, Pittman, M., Kaye, T. G., & Saitta, E. T. (2023). Sediment-encased pressure–temperature maturation experiments elucidate the impact of diagenesis on melanin-based fossil colour and its palaeobiological implications. *Paleobiology*, 1–21.

- **Roy, A.**, Rogers, C. S., Clements, T., Pittman, M., Habimana, O., Martin, P., & Vinther, J. (2020). Fossil microbodies are melanosomes: evaluating and rejecting the 'fossilised decay-associated microbes' hypothesis. *Bulletin of the American Museum of Natural History* **440**: 251–276.

- Dececchi, T.A., **Roy, A.**, Pittman, M., Kaye, T.G., Xu, X., Habib, M., Larsson, H., Wang, X., & Zheng, X. (2020). Aerodynamics show bat-winged theropods were a poor gliding dead-end. *iScience*, 101574.

- **Roy, A.**, Pittman, M., Saitta, E. T., Kaye, T. G., & Xu, X. (2019). Recent advances in amniote palaeocolour reconstruction and a framework for future research. *Biological Reviews* **95**: 22–50.

### Preprints & Submitted

- **Roy, A.**, Ghosh, P., Benson, R.J., Weston, F., Hartley, B., Salili-James, A., Poon, S.T.S., Walsh, S.A., Maidment, S., & Butler, R.J. (2026). Breaking the Bottleneck: Fully-automated CT Segmentation of Fossils using Self-Supervised Deep Learning. *Submitted to Nature Machine Intelligence.*

- **Roy, A.**, Pittman, M., Musa, M., Al-Kindi, S., Kaye, T. G., & Saitta, E. T. (2026). A multi-spectroscopic investigation into the diagenesis of avian polyene pigments: simulated maturation, chemical pathways, and palaeontological implications. *Scientific Reports* (In Review). Preprint: *Research Square* 10.21203/rs.3.rs-7900994/v1.

### Citation Metrics (Google Scholar)

| Metric | Cumulative | Since 2021 |
| --- | --- | --- |
| Raw citations | 96 | 87 |
| h-index | 4 | 4 |
| i10-index | 3 | 3 |

---

## Selected Talks & Conference Presentations

- **Roy, A.** (2026). From Molecules to Models: Integrating Experimental Taphonomy and AI to Resurrect Ancient Life. *Lapworth Lectures*, Lapworth Museum, University of Birmingham. *(Also delivered at IVPP, Shenyang Normal University, Nanjing Institute of Geology and Palaeontology, Nanjing University, and Yunnan University.)*

- **Roy, A.**, et al. (2025). Breaking the Bottleneck: Fully automated CT Segmentation of Fossils using Deep Learning. *Annual Meeting of the Palaeontological Association, University of Portsmouth, UK.*

- **Roy, A.**, et al. (2025). Experimental maturation of carotenoids and psittacofulvins indicates their lower preservation potential compared to melanin. *85th Annual Meeting of the Society of Vertebrate Paleontology, Birmingham, UK.* Symposium: Ancient Biomolecules.

- **Roy, A.** (2019). Recent advances in amniote palaeocolour reconstruction and a framework for future research. *79th Annual Meeting of the Society of Vertebrate Paleontology, Brisbane, Australia.* Podium Symposium: From molecules to macroevolution.

- **Roy, A.** (2018). Fossil colour reconstruction in paravian dinosaurs. *International Pennaraptoran Dinosaur Symposium, University of Hong Kong.* **Winner: Best Presentation Prize.**

---

## Research Grants & Awards

| Year | Award | Value |
| --- | --- | --- |
| 2024 | Marie Skłodowska-Curie Actions Postdoctoral Fellowship | £192,297 |
| 2022 | Palaeontological Association Career Development Grant | £2,345 |
| 2018–2019 | Hong Kong PhD Fellowship Conference Support Grant (×2) | HK$12,900 |
| 2017–2021 | Hong Kong PhD Fellowship, Research Grants Council of Hong Kong | HK$1,118,400 |
| 2018 | Jurassic Foundation Grant | US$1,650 |
| 2016 | University of Bristol Alumni Travel Award | £600 |

---

## Education & Professional Experience

- **Marie Skłodowska-Curie Actions Postdoctoral Fellow** | University of Birmingham, UK (2024–present)
  - Deep learning-based CT segmentation of fossils and the origins of major vertebrate groups.
- **Honorary Research Associate** | University of Bristol, UK (2022–2024)
  - Palaeocolour reconstruction in Mesozoic vertebrates.
- **Hong Kong PhD Fellow** | University of Hong Kong, HKSAR (2017–2022)
  - Thesis: *Preservation and taphonomy of colouration in dinosaurs and their close relatives.*
- **MSc Palaeobiology (Distinction)** | University of Bristol, UK (2015–2016)
- **Integrated BSc–MSc Biotechnology (1st Class)** | St. Xavier's College, University of Calcutta, India (2009–2014)

---

## Media & Public Engagement

**Written coverage:** New York Times, CNN World, Al Jazeera, EurekaAlert!, Yahoo! News, Phys.Org, The Wire Science India.

**Scientific consultation for feature films:** *Professor Shanku o El Dorado* (2019, dir. Sandip Ray); *Double Feluda* (2016, dir. Sandip Ray).

---

## Contact & Links

- **Email**: a.roy.2@bham.ac.uk
- **Google Scholar**: [scholar.google.com/citations?user=wfocjEUAAAAJ](https://scholar.google.com/citations?user=wfocjEUAAAAJ&hl=en)
- **ORCID**: [0000-0002-4890-6851](https://orcid.org/0000-0002-4890-6851)
- **ResearchGate**: [researchgate.net/profile/Arindam_Roy15](https://www.researchgate.net/profile/Arindam_Roy15)
- **GitHub**: [github.com/roy-arindam-1991](https://github.com/roy-arindam-1991)
- **LinkedIn**: [linkedin.com/in/arindam-roy-035876165](https://www.linkedin.com/in/arindam-roy-035876165/)
