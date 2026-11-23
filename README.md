# Anti Time Layer Echo (ATL ECHO) — Activation-Space Research for Multi-Agent AI Safety

**Independent research programme | Ongoing experimental investigation | Source code not publicly released**

## Overview

ATL ECHO is an ongoing research programme investigating whether changes in internal language-model activation dynamics can provide useful signals for safety-oriented observation of multi-agent systems. The work examines source attribution, changes in agent behavior, collective response dynamics, and privacy-aware monitoring arrangements.

This repository is a **research portfolio**, not a software distribution, benchmark release, production safety system, or claim of a finalized scientific result. It documents the questions being investigated, the evolution of experimental modules, and selected methodological considerations. The underlying research implementations remain private.

## Research questions

- Can activation-space measurements help distinguish an agent undergoing an experimentally induced objective change from other agents in a shared environment?
- Can temporal measurements contribute to identifying the likely source of a network-level behavioral deviation?
- How do changes in one agent relate to subsequent collective dynamics?
- What limitations arise when observations must cross organizational or principal trust boundaries?
- Can signals preceding observable behavior be studied without treating generic prompt differences as evidence of malicious intent?

These are **research questions**, not established capabilities.

## Research strands

### A. Source attribution and temporal activation dynamics

An experimental attribution strand studies temporal activation-space changes under controlled multi-agent scenarios, including reference comparisons and null conditions. Its development includes exploratory variations and later attempts to evaluate a fixed analysis approach on fresh scenarios. The investigation is not presented as a validated general-purpose attribution mechanism.

### B. Federated and privacy-aware observation

A related strand explores how monitoring and attribution might be structured when individual agents' internal representations should not be disclosed to a central observer. Experimental designs examine aggregation assumptions and failure cases, including missing reports and dishonest participants. Privacy and security guarantees for real deployments have **not** been established by the repository.

### C. Collective dynamics and cascade-oriented analysis

A separate strand investigates how changes in one participant may be associated with changes in other participants and in a shared multi-agent environment. Alternative measurement approaches and control designs are explored. These experiments do not establish universal prediction of cascading AI failures.

### D. Pre-behavioral activation traces

An exploratory strand examines whether internal activation signatures associated with controlled policy or instruction changes can be distinguished before corresponding behavior is observed. The work considers held-out-scenario evaluation and benign alternative-instruction controls. A signal associated with a changed instruction is **not**, by itself, proof of deception or harmful intent.

## Experimental status and evidence

The private research archive contains multiple evolving Python/Colab experimental versions across these strands. Source inspection confirms the presence of model-inference routines, experiment definitions, null/control procedures, statistical analysis logic, and result-export routines. **Code inspection alone does not verify that each experiment ran successfully or that any reported performance generalizes.**

The following result is reported from the frozen pilot configuration.

**Reported pilot result (Qwen2.5-1.5B-Instruct, layer 20, 5 agents, 6 rounds, intervention at round 3): 34/40 correct source attributions across two post-freeze validation sets (chance level: 20%).**

This corresponds to an observed source-attribution accuracy of **85%** under the reported experimental conditions. The finding is preliminary and limited to a single model scale and controlled experimental setting. Generalization across models, agent configurations, tasks, and operational environments has not been established.

The pilot result is reported as part of the ongoing research record and should not be interpreted as evidence of production-level reliability or independently replicated performance. Additional quantitative findings may be published following review of their execution context, evaluation procedures, and supporting experimental artifacts. Exploratory and confirmatory findings will be distinguished.

## Scope and limitations

- Research-stage investigations; not a completed or production-ready safety product.
- Primarily controlled, model-specific experimental settings; transfer across models, tasks, and operational environments remains open.
- Internal-state access is relevant to the investigated methods; this is not a claim of equivalent functionality for API-only black-box models.
- Attribution, monitoring, and early-warning interpretations require careful control conditions and further validation.
- Federated arrangements introduce trust and adversarial-participant assumptions that must be evaluated independently.
- No claim is made that the research detects all deceptive agents, prevents harmful outcomes, or establishes formal privacy guarantees.

## Availability and intellectual property

**The research implementation, executable experiments, model-interfacing routines, internal evaluation data, and development materials are not included in this repository.** This repository does not provide an executable reproduction package or an implementation specification.

**Related public materials:**

- **Foundational publication:** [The Origin of Dark Energy: The Role of Interactions Between Imaginary and Anti Time Dimensions](https://doi.org/10.17776/csj.1574774)
- **Researcher ORCID:** [0009-0009-8555-9690](https://orcid.org/0009-0009-8555-9690)
- **Figshare:** Openly archived simulation artifacts associated with the foundational publication. Their DOI references are provided in the published article.

The foundational publication and its associated simulation materials concern the original anti-time theoretical framework. They should not be interpreted as an independently reproducible release or validation of the ATL ECHO AI-safety experiments.

© 2026 Gizem Akıncı İşten. All rights reserved in the original materials presented here, subject to applicable law and third-party rights. Public visibility does not grant a software license, authorization to reuse unpublished source code, or permission to represent this research as a completed product. General scientific ideas and independently developed methods may be subject to different legal treatment.

## Research communication

This repository may be updated as the research develops. Any future scientific claims, publications, and data releases should be assessed by their own evidence and stated limitations. For research correspondence, use the repository's GitHub contact mechanisms.

**Status:** Ongoing research — public documentation only.
