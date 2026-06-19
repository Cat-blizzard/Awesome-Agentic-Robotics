# Awesome Agentic Robotics [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of research on **Agentic Robotics**: memory, planning, world models, verification, failure recovery, tool use, and safety for physical agents.

This repository follows a compact Awesome-list style: entries are grouped by topic and sorted by month in descending order. Each item uses the format:

`[YYYY.M] [Venue/Org] Title [paper] [project] [code]`

## Table of Contents

| Section | Description |
| --- | --- |
| [Surveys and Position Papers](#surveys-and-position-papers) | Field definitions, surveys, and position papers |
| [Agentic Robotics Architectures](#agentic-robotics-architectures) | Planner, executor, verifier, memory, and orchestration architectures |
| [Embodied Memory](#embodied-memory) | Episodic, semantic, spatial, temporal, and retrieval-based memory |
| [Planning and Reasoning](#planning-and-reasoning) | LLM/VLM planning, task decomposition, and grounded reasoning |
| [World Models and World-Action Models](#world-models-and-world-action-models) | Predictive models for planning and action generation |
| [Verification and Self-Evaluation](#verification-and-self-evaluation) | Success detection, temporal verification, and self-checking |
| [Failure Detection and Recovery](#failure-detection-and-recovery) | Failure reasoning, correction, and recovery policies |
| [Skill Calling and Tool Use for Robots](#skill-calling-and-tool-use-for-robots) | Skill libraries, robot APIs, ROS actions, and code-as-policy |
| [Long-Horizon Manipulation](#long-horizon-manipulation) | Long-horizon, compositional, and progress-aware manipulation |
| [Embodied Navigation Agents](#embodied-navigation-agents) | VLN, open-vocabulary navigation, and multi-robot navigation |
| [Human-Robot Interaction and Dialogue Agents](#human-robot-interaction-and-dialogue-agents) | Dialogue, mixed initiative, feedback, and human modeling |
| [Safety, Governance, and Physical Risk](#safety-governance-and-physical-risk) | Guardrails, governance, consent, and runtime constraints |
| [Benchmarks, Simulators, and Datasets](#benchmarks-simulators-and-datasets) | Evaluation resources for agentic robot behavior |
| [Open-Source Systems and Frameworks](#open-source-systems-and-frameworks) | Open models, codebases, and robot agent frameworks |
| [Industrial Signals and Technical Reports](#industrial-signals-and-technical-reports) | Technical reports, product signals, and industry releases |
| [Related Awesome Lists](#related-awesome-lists) | Adjacent curated lists |

**Paper ordering:** within each topic, entries use `[YYYY.M]` and are sorted newest first.

---

## Surveys and Position Papers

> Field definitions, surveys, and position papers for Agentic Robotics.

### 2026

- [2026.5] World Action Models: The Next Frontier in Embodied AI [[paper]](https://arxiv.org/abs/2605.12090)
- [2026.5] World Model for Robot Learning: A Comprehensive Survey [[paper]](https://arxiv.org/abs/2605.00080)
- [2026.4] Vision-Language-Action Safety: Threats, Challenges, Evaluations, and Mechanisms [[paper]](https://arxiv.org/abs/2604.23775)

### 2025

- [2025.8] Towards Embodied Agentic AI: Review and Classification of LLM- and VLM-Driven Robot Autonomy and Interaction [[paper]](https://arxiv.org/abs/2508.05294)
- [2025.8] Agentic LLM-based robotic systems for real-world applications [[paper]](https://www.frontiersin.org/journals/robotics-and-ai/articles/10.3389/frobt.2025.1605405/full)

### 2023

- [2023.11] Large Language Models for Robotics: A Survey [[paper]](https://arxiv.org/html/2311.07226v2)

---

## Agentic Robotics Architectures

> Architectures that combine reasoning, execution, verification, memory, skill selection, or multi-agent coordination.

### 2026

- [2026.3] RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks [[paper]](https://arxiv.org/abs/2603.11558)

### 2025

- [2025.10] Gemini Robotics 1.5: Pushing the Frontier of Generalist Robots with Advanced Embodied Reasoning, Thinking, and Motion Transfer [[paper]](https://arxiv.org/abs/2510.03342)
- [2025.5] Agentic Robot: A Brain-Inspired Framework for Vision-Language-Action Models in Embodied Agents [[paper]](https://arxiv.org/abs/2505.23450)
- [2025.2] Hi Robot: Open-Ended Instruction Following with Hierarchical Vision-Language-Action Models [[paper]](https://arxiv.org/html/2502.19417v1) [[project]](https://www.pi.website/research/hirobot)

### 2023

- [2023.9] SMART-LLM: Smart Multi-Agent Robot Task Planning using Large Language Models [[paper]](https://arxiv.org/abs/2309.10062)

### 2022

- [2022.4] Do As I Can, Not As I Say: Grounding Language in Robotic Affordances [[paper]](https://arxiv.org/abs/2204.01691) [[project]](https://say-can.github.io/)

---

## Embodied Memory

> Memory systems for physical agents: working memory, memory banks, semantic-spatial memory, scene memory, and embodied retrieval.

### 2026

- [2026.6] eMEM: A Hybrid Spatio-Temporal Memory System For Embodied Agents [[paper]](https://arxiv.org/abs/2606.03374)
- [2026.4] HELM: Harness-Enhanced Long-horizon Memory for Vision-Language-Action Manipulation [[paper]](https://arxiv.org/abs/2604.18791)
- [2026.3] Chameleon: Episodic Memory for Long-Horizon Robotic Manipulation [[paper]](https://arxiv.org/abs/2603.24576)
- [2026.3] ReMem-VLA: Empowering Vision-Language-Action Model with Memory via Dual-Level Recurrent Queries [[paper]](https://arxiv.org/abs/2603.12942)
- [2026.3] MEM: Multi-Scale Embodied Memory for Vision Language Action Models [[paper]](https://www.pi.website/download/Mem.pdf) [[project]](https://www.pi.website/research/memory)

### 2025

- [2025.11] EchoVLA: Robotic Vision-Language-Action Model with Synergistic Declarative Memory for Mobile Manipulation [[paper]](https://arxiv.org/abs/2511.18112)
- [2025.11] Searching in Space and Time: Unified Memory-Action Loops for Open-World Object Retrieval [[paper]](https://arxiv.org/abs/2511.14004) [[project]](https://amrl.cs.utexas.edu/STAR/)
- [2025.10] MemER: Scaling Up Memory for Robot Control via Experience Retrieval [[paper]](https://arxiv.org/abs/2510.20328) [[project]](https://jen-pan.github.io/memer/)
- [2025.9] Meta-Memory: Retrieving and Integrating Semantic-Spatial Memories for Robot Spatial Reasoning [[paper]](https://arxiv.org/abs/2509.20754)
- [2025.8] MemoryVLA: Perceptual-Cognitive Memory in Vision-Language-Action Models for Robotic Manipulation [[paper]](https://arxiv.org/abs/2508.19236)
- [2025.8] RoboMemory: A Brain-inspired Multi-memory Agentic Framework for Lifelong Learning in Physical Embodied Systems [[paper]](https://arxiv.org/abs/2508.01415)

### 2024

- [2024.11] [CVPR 25] 3D-Mem: 3D Scene Memory for Embodied Exploration and Reasoning [[paper]](https://arxiv.org/abs/2411.17735) [[project]](https://umass-embodied-agi.github.io/3D-Mem/) [[code]](https://github.com/UMass-Embodied-AGI/3D-Mem)
- [2024.11] DynaMem: Online Dynamic Spatio-Semantic Memory for Open World Mobile Manipulation [[paper]](https://arxiv.org/abs/2411.04999) [[project]](https://dynamem.github.io/)
- [2024.9] Embodied-RAG: General Non-parametric Embodied Memory for Retrieval and Generation [[paper]](https://arxiv.org/html/2409.18313v2)

---

## Planning and Reasoning

> LLM/VLM-based planning, grounded reasoning, task decomposition, value maps, and closed-loop feedback.

### 2023

- [2023.7] VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models [[paper]](https://arxiv.org/abs/2307.05973) [[project]](https://voxposer.github.io/)

### 2022

- [2022.12] LLM-Planner: Few-Shot Grounded Planning for Embodied Agents with Large Language Models [[paper]](https://arxiv.org/abs/2212.04088)
- [2022.9] ProgPrompt: Generating Situated Robot Task Plans using Large Language Models [[paper]](https://arxiv.org/abs/2209.11302)
- [2022.7] Inner Monologue: Embodied Reasoning through Planning with Language Models [[paper]](https://arxiv.org/abs/2207.05608)
- [2022.4] SayCan: Grounding Language in Robotic Affordances [[paper]](https://arxiv.org/abs/2204.01691) [[project]](https://say-can.github.io/)
- [2022.1] Language Models as Zero-Shot Planners: Extracting Actionable Knowledge for Embodied Agents [[paper]](https://arxiv.org/abs/2201.07207)

---

## World Models and World-Action Models

> Predictive models that support future imagination, control, action synthesis, and internal planning.

### 2026

- [2026.6] World-Language-Action Model for Unified World Modeling, Language Reasoning, and Action Synthesis [[paper]](https://arxiv.org/abs/2606.05979)
- [2026.5] World Action Models: The Next Frontier in Embodied AI [[paper]](https://arxiv.org/abs/2605.12090)
- [2026.5] World Model for Robot Learning: A Comprehensive Survey [[paper]](https://arxiv.org/abs/2605.00080)
- [2026.2] World Action Models are Zero-shot Policies [[paper]](https://arxiv.org/html/2602.15922v1)

### 2025

- [2025.6] V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning [[paper]](https://arxiv.org/abs/2506.09985)

### 2023

- [2023.10] TD-MPC2: Scalable, Robust World Models for Continuous Control [[paper]](https://arxiv.org/abs/2310.16828)

---

## Verification and Self-Evaluation

> Success detection, temporal verification, execution checking, and safety-aware evaluation.

### 2025

- [2025.12] Guardian: Detecting Robotic Planning and Execution Errors with Vision-Language Models [[paper]](https://arxiv.org/abs/2512.01946)
- [2025.5] Agentic Robot: A Brain-Inspired Framework for Vision-Language-Action Models in Embodied Agents [[paper]](https://arxiv.org/abs/2505.23450)
- [2025.3] RoboGuard: Safety Guardrails for LLM-Enabled Robots [[paper]](https://arxiv.org/abs/2503.07885) [[code]](https://github.com/KumarRobotics/RoboGuard)

### 2024

- [2024.10] AHA: A Vision-Language-Model for Detecting and Reasoning Over Failures in Robotic Manipulation [[paper]](https://arxiv.org/abs/2410.00371)
- [2024.3] [AAAI] Vision-Language Models for Robot Success Detection [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/30552/32714)

### 2023

- [2023.3] Vision-Language Models as Success Detectors [[paper]](https://arxiv.org/abs/2303.07280)

---

## Failure Detection and Recovery

> Failure detection, natural-language failure reasoning, motion correction, task-level recovery, and safe takeover.

### 2026

- [2026.2] ARMOR: Self-Refining Vision Language Model for Robotic Failure Detection and Reasoning [[paper]](https://arxiv.org/html/2602.12405v1)

### 2025

- [2025.12] Guardian: Detecting Robotic Planning and Execution Errors with Vision-Language Models [[paper]](https://arxiv.org/abs/2512.01946)
- [2025.10] FailSafe-VLM: Reasoning and Recovery from Failures in Vision-Language-Action Models [[paper]](https://arxiv.org/html/2510.01642v1)
- [2025.3] A Unified Framework for Real-Time Failure Handling in Autonomous Robots [[paper]](https://arxiv.org/html/2503.15202v2)

### 2024

- [2024.10] AHA: A Vision-Language-Model for Detecting and Reasoning Over Failures in Robotic Manipulation [[paper]](https://arxiv.org/abs/2410.00371)
- [2024.9] Automating Robot Failure Recovery Using Vision-Language Models [[paper]](https://arxiv.org/abs/2409.03966)

---

## Skill Calling and Tool Use for Robots

> Robot-specific tool use: skill libraries, controller APIs, ROS actions, behavior trees, state machines, and code-as-policy.

### 2025

- [2025.5] RAI: Flexible Agent Framework for Embodied AI [[paper]](https://arxiv.org/abs/2505.07532) [[code]](https://github.com/RobotecAI/rai)

### 2024

- [2024.6] ROS-LLM: A ROS framework for embodied AI with task feedback and structured reasoning [[paper]](https://arxiv.org/abs/2406.19741)

### 2023

- [2023.7] VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models [[paper]](https://arxiv.org/abs/2307.05973) [[project]](https://voxposer.github.io/)

### 2022

- [2022.9] ProgPrompt: Generating Situated Robot Task Plans using Large Language Models [[paper]](https://arxiv.org/abs/2209.11302)
- [2022.9] Code as Policies: Language Model Programs for Embodied Control [[paper]](https://arxiv.org/abs/2209.07753)
- [2022.4] SayCan: Grounding Language in Robotic Affordances [[paper]](https://arxiv.org/abs/2204.01691) [[project]](https://say-can.github.io/)

---

## Long-Horizon Manipulation

> Long-horizon, compositional, memory-conditioned, and progress-aware manipulation.

### 2026

- [2026.4] HELM: Harness-Enhanced Long-horizon Memory for Vision-Language-Action Manipulation [[paper]](https://arxiv.org/abs/2604.18791)
- [2026.3] Chameleon: Episodic Memory for Long-Horizon Robotic Manipulation [[paper]](https://arxiv.org/abs/2603.24576)
- [2026.3] RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks [[paper]](https://arxiv.org/abs/2603.11558)

### 2025

- [2025.10] MemER: Scaling Up Memory for Robot Control via Experience Retrieval [[paper]](https://arxiv.org/abs/2510.20328) [[project]](https://jen-pan.github.io/memer/)
- [2025.8] MemoryVLA: Perceptual-Cognitive Memory in Vision-Language-Action Models for Robotic Manipulation [[paper]](https://arxiv.org/abs/2508.19236)
- [2025.4] pi0.5: a Vision-Language-Action Model with Open-World Generalization [[paper]](https://arxiv.org/abs/2504.16054)

### 2024

- [2024.10] pi0: A Vision-Language-Action Flow Model for General Robot Control [[paper]](https://arxiv.org/abs/2410.24164)
- [2024.6] OpenVLA: An Open-Source Vision-Language-Action Model [[paper]](https://arxiv.org/abs/2406.09246) [[code]](https://github.com/openvla/openvla)

### 2023

- [2023.4] Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware [[paper]](https://arxiv.org/abs/2304.13705)
- [2023.3] Diffusion Policy: Visuomotor Policy Learning via Action Diffusion [[paper]](https://arxiv.org/abs/2303.04137)

### 2021

- [2021.12] CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks [[paper]](https://arxiv.org/abs/2112.03227)

---

## Embodied Navigation Agents

> VLN, open-vocabulary navigation, lifelong navigation, social navigation, and cooperative multi-robot navigation.

### 2025

- [2025.11] Searching in Space and Time: Unified Memory-Action Loops for Open-World Object Retrieval [[paper]](https://arxiv.org/abs/2511.14004) [[project]](https://amrl.cs.utexas.edu/STAR/)

### 2024

- [2024.12] [RSS 25] Uni-NaVid: A Video-based Vision-Language-Action Model for Unifying Embodied Navigation Tasks [[paper]](https://arxiv.org/abs/2412.06224) [[project]](https://pku-epic.github.io/Uni-NaVid/)
- [2024.11] [CVPR 25] 3D-Mem: 3D Scene Memory for Embodied Exploration and Reasoning [[paper]](https://arxiv.org/abs/2411.17735) [[project]](https://umass-embodied-agi.github.io/3D-Mem/) [[code]](https://github.com/UMass-Embodied-AGI/3D-Mem)
- [2024.11] DynaMem: Online Dynamic Spatio-Semantic Memory for Open World Mobile Manipulation [[paper]](https://arxiv.org/abs/2411.04999) [[project]](https://dynamem.github.io/)
- [2024.4] GOAT-Bench: A Benchmark for Multi-Modal Lifelong Navigation [[paper]](https://arxiv.org/abs/2404.06609)
- [2024.4] VLM-Social-Nav: Socially Aware Robot Navigation through Scoring Using Vision-Language Models [[paper]](https://arxiv.org/html/2404.00210v1)
- [2024.2] Vision-Language Navigation with Embodied Intelligence [[paper]](https://arxiv.org/html/2402.14304v1)

### 2023

- [2023.10] Co-NavGPT: Multi-Robot Cooperative Visual Semantic Navigation using Large Language Models [[paper]](https://arxiv.org/abs/2310.07937)

### 2022

- [2022.7] LM-Nav: Robotic Navigation with Large Pre-Trained Models of Language, Vision, and Action [[paper]](https://arxiv.org/abs/2207.04429)

### 2018

- [2018.6] [CVPR] Vision-and-Language Navigation: Interpreting Visually-Grounded Navigation Instructions in Real Environments [[paper]](https://openaccess.thecvf.com/content_cvpr_2018/papers/Anderson_Vision-and-Language_Navigation_Interpreting_CVPR_2018_paper.pdf)

---

## Human-Robot Interaction and Dialogue Agents

> Human feedback, dialogue management, mixed initiative, social robot planning, and human-in-the-loop coordination.

### 2025

- [2025.8] MICoBot: Mixed-Initiative Dialog for Human-Robot Collaborative Manipulation [[paper]](https://arxiv.org/html/2508.05535v1)

### 2024

- [2024.5] Leveraging Large Language Models in Human-Robot Interaction [[paper]](https://arxiv.org/html/2405.00693v2)
- [2024.2] Conversational Language Models for Human-in-the-Loop Multi-Robot Coordination [[paper]](https://arxiv.org/abs/2402.19166)
- [2024.1] Understanding LLM-powered Human-Robot Interaction [[paper]](https://arxiv.org/abs/2401.03217)

### 2023

- [2023.7] A Survey on Dialogue Management in Human-Robot Interaction [[paper]](https://arxiv.org/abs/2307.10897)
- [2023.3] Large Language Models as Zero-Shot Human Models for Human-Robot Interaction [[paper]](https://arxiv.org/abs/2303.03548)

### 2022

- [2022.7] Inner Monologue: Embodied Reasoning through Planning with Language Models [[paper]](https://arxiv.org/abs/2207.05608)

---

## Safety, Governance, and Physical Risk

> Safety guardrails, policy-constrained execution, governance benchmarks, consent, delegation, and physical irreversibility.

### 2026

- [2026.5] Consent Chain Degradation in Embodied Multi-Agent Systems [[paper]](https://arxiv.org/html/2605.16300v1)
- [2026.4] Vision-Language-Action Safety: Threats, Challenges, Evaluations, and Mechanisms [[paper]](https://arxiv.org/abs/2604.23775)
- [2026.4] EmbodiedGovBench: A Benchmark for Governance-Constrained Embodied Agents [[paper]](https://arxiv.org/html/2604.11174v1)
- [2026.4] Harnessing Embodied Agents: Runtime Governance for Policy-Constrained Execution [[paper]](https://arxiv.org/abs/2604.07833)

### 2025

- [2025.3] RoboGuard: Safety Guardrails for LLM-Enabled Robots [[paper]](https://arxiv.org/abs/2503.07885) [[code]](https://github.com/KumarRobotics/RoboGuard)

---

## Benchmarks, Simulators, and Datasets

> Benchmarks and datasets for long-horizon tasks, memory, recovery, navigation, multi-robot systems, and safety.

### 2026

- [2026.3] RoboCasa365: A Large-Scale Simulation Framework for Generalist Robot Policies [[paper]](https://arxiv.org/html/2603.04356v1)

### 2025

- [2025.4] RoboTwin: Dual-Arm Robot Benchmark with Generative Digital Twins [[paper]](https://arxiv.org/abs/2504.13059)

### 2024

- [2024.6] RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots [[paper]](https://arxiv.org/abs/2406.02523)
- [2024.4] GOAT-Bench: A Benchmark for Multi-Modal Lifelong Navigation [[paper]](https://arxiv.org/abs/2404.06609)

### 2023

- [2023.10] Habitat 3.0: A Co-Habitat for Humans, Avatars and Robots [[paper]](https://arxiv.org/abs/2310.13724)
- [2023.10] Open X-Embodiment: Robotic Learning Datasets and RT-X Models [[paper]](https://arxiv.org/abs/2310.08864) [[code]](https://github.com/google-deepmind/open_x_embodiment)
- [2023.8] BridgeData V2: A Dataset for Robot Learning at Scale [[paper]](https://arxiv.org/abs/2308.12952)
- [2023.6] LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning [[paper]](https://arxiv.org/abs/2306.03310)

### 2021

- [2021.12] CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks [[paper]](https://arxiv.org/abs/2112.03227)

---

## Open-Source Systems and Frameworks

> Open models, robot agent frameworks, simulation systems, benchmark codebases, and data infrastructure.

### 2025

- [2025.5] RAI: Flexible Agent Framework for Embodied AI [[paper]](https://arxiv.org/abs/2505.07532) [[code]](https://github.com/RobotecAI/rai)

### 2024

- [2024.11] [CVPR 25] 3D-Mem [[paper]](https://arxiv.org/abs/2411.17735) [[project]](https://umass-embodied-agi.github.io/3D-Mem/) [[code]](https://github.com/UMass-Embodied-AGI/3D-Mem)
- [2024.6] ROS-LLM: A ROS framework for embodied AI with task feedback and structured reasoning [[paper]](https://arxiv.org/abs/2406.19741)
- [2024.6] OpenVLA: An Open-Source Vision-Language-Action Model [[paper]](https://arxiv.org/abs/2406.09246) [[code]](https://github.com/openvla/openvla)
- [2024.6] RoboCasa [[paper]](https://arxiv.org/abs/2406.02523)
- [2024.5] Octo: An Open-Source Generalist Robot Policy [[paper]](https://arxiv.org/abs/2405.12213)

### 2023

- [2023.11] RoboFlamingo: Vision-Language Foundation Models as Effective Robot Imitators [[paper]](https://arxiv.org/abs/2311.01378)
- [2023.10] Open X-Embodiment [[code]](https://github.com/google-deepmind/open_x_embodiment)

---

## Industrial Signals and Technical Reports

> Technical reports, model releases, product signals, and industrial systems that point toward deployable physical agents.

### 2025

- [2025.10] [Google DeepMind] Gemini Robotics 1.5 [[paper]](https://arxiv.org/abs/2510.03342)
- [2025.4] [Physical Intelligence] pi0.5: a Vision-Language-Action Model with Open-World Generalization [[paper]](https://arxiv.org/abs/2504.16054)
- [2025.3] [Google DeepMind] Gemini Robotics: Bringing AI into the Physical World [[paper]](https://arxiv.org/abs/2503.20020)
- [2025.3] [NVIDIA] GR00T N1: An Open Foundation Model for Generalist Humanoid Robots [[paper]](https://arxiv.org/abs/2503.14734) [[code]](https://github.com/Nvidia/Isaac-GR00T)
- [2025.2] [Physical Intelligence] Hi Robot [[project]](https://www.pi.website/research/hirobot)
- [2025.2] [Figure] Helix [[project]](https://www.figure.ai/news/helix)

### 2024

- [2024.10] [Physical Intelligence] pi0: A Vision-Language-Action Flow Model for General Robot Control [[paper]](https://arxiv.org/abs/2410.24164)

---

## Related Awesome Lists

- [Awesome Memory for Robotics](https://github.com/Everloom-129/Awesome-Memory-for-Robotics) - A focused list on memory systems, memory-augmented policies, spatial memory, and memory benchmarks for robotics.

---

## Contributing

Contributions are welcome. Please keep the list focused on agentic robotics instead of general robotics papers.

Good entries should clearly relate to at least one of:

- embodied memory
- planning and reasoning
- world models or world-action models
- verification and self-evaluation
- failure detection and recovery
- skill calling, tool use, or robot APIs
- long-horizon manipulation
- embodied navigation
- human-robot interaction
- safety, governance, or physical risk
- benchmarks that evaluate agentic robot behavior

Please include concise links such as `[paper]`, `[project]`, `[code]`, `[blog]`, or `[report]`.
