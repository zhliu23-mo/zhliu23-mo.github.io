---
title: "NeRM-Net: Reflective Evolution of Routing Strategies for Dynamic Communication Networks"
collection: publications
published: true
category: conferences
permalink: /publication/2025-09-01-NeRM-Net
excerpt: 'We propose a reflective co-evolutionary framework that optimizes task descriptions and routing algorithms via network state feedback using LLMs.'
date: 2025-09-01
venue: 'ACM CoNEXT 2025 Workshop'
paperurl: 'https://dl.acm.org/doi/epdf/10.1145/3769697.3771243'
DOI: 'https://doi.org/10.1145/3769697.3771243'
citation: 'Guo, Shuhan and Yin, Nan and Liu, Shuzhi and Liu, Zhongheng and Huangfu, Wei and Yao, Quanming. (2025). &quot;"NeRM-Net: Reflective Evolution of Routing Strategies for Dynamic Communication Networks."&quot; <i>ACM CoNEXT Workshop</i>.'

---
## Background

Dynamic communication networks with topological changes and multi-dimensional constraints (bandwidth, latency, compute) pose significant routing challenges.

## Contribution

* Proposed a **reflective co-evolutionary framework** that optimizes task descriptions and routing algorithms via network state feedback.
* Conducted extensive baseline experiments and ablation studies.
* Demonstrated superior performance over Optimal and ACO baselines, improving flow acceptance rate by up to **57.49%** in 100-flow scenarios.

[Download PDF here](https://dl.acm.org/doi/epdf/10.1145/3769697.3771243)


# Cite our paper

```latex
@inproceedings{10.1145/3769697.3771243,
author = {Guo, Shuhan and Yin, Nan and Liu, Shuzhi and Liu, Zhongheng and Huangfu, Wei and Yao, Quanming},
title = {NeRM-Net: Reflective Evolution of Routing Strategies for Dynamic Communication Networks},
year = {2025},
isbn = {9798400722431},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3769697.3771243},
doi = {10.1145/3769697.3771243},
abstract = {Modern networks demand routing strategies that jointly optimize heterogeneous constraints like bandwidth, latency, and compute resources. While LLM-driven algorithm generation excels in static domains, it struggles in dynamic network environments where these constraints are interdependent and topology-aware. We introduce NeRM-Net, a reflective co-evolution framework that jointly optimizes task specifications and routing algorithms through network-aware feedback. At its core, an adaptive environmental feedback module captures dynamic network states and performance outcomes. This module steers two complementary processes: (i) structure-conditioned prompt evolution, which aligns problem descriptions with graph-level constraints for more effective guidance, and (ii) feasibility-guided algorithm refinement, which evolves routing logic by analyzing constraint violations to improve solution quality. Experiments on Abilene and GEANT topologies show NeRM-Net consistently outperforms baselines in flow acceptance and resource efficiency, demonstrating its effectiveness and scalability.},
booktitle = {Proceedings of the ACM Conext-2025 Workshop on the Polymorphic Network},
pages = {32–38},
numpages = {7},
keywords = {network strategy optimization, resource-constrained routing, llm-driven algorithm evolution},
location = {Hong Kong},
series = {PN '25}
}
```
