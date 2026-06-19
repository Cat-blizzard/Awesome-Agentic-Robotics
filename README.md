# Awesome Agentic Robotics

Memory, planning, world models, verification, failure recovery, and safety for physical agents.

This repository curates papers, technical reports, benchmarks, datasets, and open-source systems that help define **Agentic Robotics**: robot systems that can reason over tasks, maintain embodied memory, call skills and tools, verify progress, recover from failures, and operate under physical safety constraints.

The v0.1 list is intentionally selective. Each section starts with a small seed set of works that help define the problem boundary instead of becoming a generic VLA paper dump.

## Contents

- [Surveys and Position Papers](#surveys-and-position-papers)
- [Agentic Robotics Architectures](#agentic-robotics-architectures)
- [Embodied Memory](#embodied-memory)
- [Planning and Reasoning](#planning-and-reasoning)
- [World Models and World-Action Models](#world-models-and-world-action-models)
- [Verification and Self-Evaluation](#verification-and-self-evaluation)
- [Failure Detection and Recovery](#failure-detection-and-recovery)
- [Skill Calling and Tool Use for Robots](#skill-calling-and-tool-use-for-robots)
- [Long-Horizon Manipulation](#long-horizon-manipulation)
- [Embodied Navigation Agents](#embodied-navigation-agents)
- [Human-Robot Interaction and Dialogue Agents](#human-robot-interaction-and-dialogue-agents)
- [Safety, Governance, and Physical Risk](#safety-governance-and-physical-risk)
- [Benchmarks, Simulators, and Datasets](#benchmarks-simulators-and-datasets)
- [Open-Source Systems and Frameworks](#open-source-systems-and-frameworks)
- [Industrial Signals and Technical Reports](#industrial-signals-and-technical-reports)
- [Contributing](#contributing)

## Surveys and Position Papers

**Why this matters for Agentic Robotics:** these works frame the field and distinguish agentic robotics from general robot learning, embodied AI, and VLA model collections.

- [Towards Embodied Agentic AI: Review and Classification of LLM- and VLM-Driven Robot Autonomy and Interaction](https://arxiv.org/abs/2508.05294) - A direct fit for defining LLM/VLM-driven agentic robot autonomy.
- [Agentic LLM-based robotic systems for real-world applications](https://www.frontiersin.org/journals/robotics-and-ai/articles/10.3389/frobt.2025.1605405/full) - Focuses on real-world robotic systems, agenticness, and ethics.
- [Large Language Models for Robotics: A Survey](https://arxiv.org/html/2311.07226v2) - A broad entry point for LLMs in robotics.
- [World Action Models: The Next Frontier in Embodied AI](https://arxiv.org/abs/2605.12090) - Frames world-action modeling as a bridge between world models and action generation.
- [World Model for Robot Learning: A Comprehensive Survey](https://arxiv.org/abs/2605.00080) - Surveys world models for robot learning.
- [Vision-Language-Action Safety: Threats, Challenges, Evaluations, and Mechanisms](https://arxiv.org/abs/2604.23775) - Surveys safety problems specific to VLA systems.

## Agentic Robotics Architectures

**Why this matters for Agentic Robotics:** architecture is where planning, execution, verification, memory, and skill orchestration become a robot agent rather than a single policy.

- [Agentic Robot: A Brain-Inspired Framework for Vision-Language-Action Models in Embodied Agents](https://arxiv.org/abs/2505.23450) - Explicitly combines a reasoning model, VLA executor, and temporal verifier.
- [Gemini Robotics 1.5: Pushing the Frontier of Generalist Robots with Advanced Embodied Reasoning, Thinking, and Motion Transfer](https://arxiv.org/abs/2510.03342) - An industrial-scale signal for embodied reasoning plus VLA architecture.
- [Hi Robot: Open-Ended Instruction Following with Hierarchical Vision-Language-Action Models](https://arxiv.org/html/2502.19417v1) - A hierarchical high-level VLM and low-level VLA system.
- [Do As I Can, Not As I Say: Grounding Language in Robotic Affordances](https://arxiv.org/abs/2204.01691) - A classic starting point for LLM planning grounded by value and affordance estimates.
- [RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks](https://arxiv.org/abs/2603.11558) - Covers agentic data collection, policy refinement, and long-horizon execution.
- [SMART-LLM: Smart Multi-Agent Robot Task Planning using Large Language Models](https://arxiv.org/abs/2309.10062) - A representative multi-robot task planning system.

## Embodied Memory

**Why this matters for Agentic Robotics:** memory lets physical agents move beyond reactive policies by grounding decisions in past observations, spatial context, task history, and long-term experience.

- [MemoryVLA: Perceptual-Cognitive Memory in Vision-Language-Action Models for Robotic Manipulation](https://arxiv.org/abs/2508.19236) - Combines working memory, a memory bank, and a diffusion action expert.
- [RoboMemory: A Brain-inspired Multi-memory Agentic Framework for Lifelong Learning in Physical Embodied Systems](https://arxiv.org/abs/2508.01415) - Covers spatial, temporal, episodic, and semantic memory.
- [Meta-Memory: Retrieving and Integrating Semantic-Spatial Memories for Robot Spatial Reasoning](https://arxiv.org/abs/2509.20754) - Focuses on semantic-spatial memory retrieval and integration.
- [EchoVLA: Robotic Vision-Language-Action Model with Synergistic Declarative Memory for Mobile Manipulation](https://arxiv.org/abs/2511.18112) - Uses scene memory and episodic memory for long-horizon mobile manipulation.
- [eMEM: A Hybrid Spatio-Temporal Memory System For Embodied Agents](https://arxiv.org/abs/2606.03374) - A graph-structured, multi-index spatio-temporal memory system.
- [Embodied-RAG: General Non-parametric Embodied Memory for Retrieval and Generation](https://arxiv.org/html/2409.18313v2) - Recasts retrieval-augmented generation as embodied memory.

## Planning and Reasoning

**Why this matters for Agentic Robotics:** planning and reasoning connect language goals to executable, grounded, and constraint-aware behavior in the physical world.

- [Language Models as Zero-Shot Planners: Extracting Actionable Knowledge for Embodied Agents](https://arxiv.org/abs/2201.07207) - An early classic for high-level action decomposition with language models.
- [LLM-Planner: Few-Shot Grounded Planning for Embodied Agents with Large Language Models](https://arxiv.org/abs/2212.04088) - Studies few-shot grounded planning for embodied agents.
- [ProgPrompt: Generating Situated Robot Task Plans using Large Language Models](https://arxiv.org/abs/2209.11302) - Uses program-like prompts to generate executable task plans.
- [SayCan: Grounding Language in Robotic Affordances](https://say-can.github.io/) - Combines language likelihood with robot affordance and value estimates.
- [Inner Monologue: Embodied Reasoning through Planning with Language Models](https://arxiv.org/abs/2207.05608) - Integrates scene descriptions, success detection, and human feedback into closed-loop reasoning.
- [VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models](https://arxiv.org/abs/2307.05973) - Generates 3D value maps for downstream motion planning.

## World Models and World-Action Models

**Why this matters for Agentic Robotics:** world models give robot agents internal predictive structure, making planning, counterfactual reasoning, and long-horizon control more agentic.

- [World Action Models: The Next Frontier in Embodied AI](https://arxiv.org/abs/2605.12090) - A top-level reference for the world-action model direction.
- [World Model for Robot Learning: A Comprehensive Survey](https://arxiv.org/abs/2605.00080) - Surveys world models in robot learning.
- [V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning](https://arxiv.org/abs/2506.09985) - Connects video self-supervision to prediction, planning, and robotics.
- [TD-MPC2: Scalable, Robust World Models for Continuous Control](https://arxiv.org/abs/2310.16828) - A strong latent world model plus MPC baseline for continuous control.
- [World Action Models are Zero-shot Policies](https://arxiv.org/html/2602.15922v1) - Uses WAMs to predict future world states and actions.
- [World-Language-Action Model for Unified World Modeling, Language Reasoning, and Action Synthesis](https://arxiv.org/abs/2606.05979) - Unifies world modeling, language reasoning, and action synthesis.

## Verification and Self-Evaluation

**Why this matters for Agentic Robotics:** physical agents need ways to judge whether an action or plan worked before continuing, retrying, asking for help, or stopping safely.

- [Vision-Language Models as Success Detectors](https://arxiv.org/abs/2303.07280) - Frames success detection as a VQA or reward modeling problem.
- [Vision-Language Models for Robot Success Detection](https://ojs.aaai.org/index.php/AAAI/article/view/30552/32714) - Applies VLM-style classification to robot success detection.
- [Agentic Robot: A Brain-Inspired Framework for Vision-Language-Action Models in Embodied Agents](https://arxiv.org/abs/2505.23450) - Includes a temporal verifier for checking execution progress.
- [AHA: A Vision-Language-Model for Detecting and Reasoning Over Failures in Robotic Manipulation](https://arxiv.org/abs/2410.00371) - Treats failure reasoning as part of verification.
- [Guardian: Detecting Robotic Planning and Execution Errors with Vision-Language Models](https://arxiv.org/abs/2512.01946) - Studies multi-view planning and execution error detection.
- [RoboGuard: Safety Guardrails for LLM-Enabled Robots](https://arxiv.org/abs/2503.07885) - Moves verification toward safety constraints and guardrails.

## Failure Detection and Recovery

**Why this matters for Agentic Robotics:** robust robot agents must detect execution failures, explain them, and recover instead of blindly continuing a failed plan.

- [AHA: A Vision-Language-Model for Detecting and Reasoning Over Failures in Robotic Manipulation](https://arxiv.org/abs/2410.00371) - Detects manipulation failures and produces natural-language failure reasoning.
- [Guardian: Detecting Robotic Planning and Execution Errors with Vision-Language Models](https://arxiv.org/abs/2512.01946) - Synthesizes failure data and trains VLMs for planning and execution error detection.
- [Automating Robot Failure Recovery Using Vision-Language Models](https://arxiv.org/abs/2409.03966) - Uses VLMs for motion-level correction and task-level recovery.
- [A Unified Framework for Real-Time Failure Handling in Autonomous Robots](https://arxiv.org/html/2503.15202v2) - Combines VLMs, reactive planning, and behavior trees for real-time failure handling.
- [ARMOR: Self-Refining Vision Language Model for Robotic Failure Detection and Reasoning](https://arxiv.org/html/2602.12405v1) - Uses iterative self-refinement for failure reasoning.
- [FailSafe-VLM](https://arxiv.org/html/2510.01642v1) - Monitors VLA execution, detects potential failures, and proposes recovery actions.

## Skill Calling and Tool Use for Robots

**Why this matters for Agentic Robotics:** robots become agents when they can select skills, call controllers, use APIs, and compose tools instead of only emitting low-level actions.

- [SayCan: Grounding Language in Robotic Affordances](https://say-can.github.io/) - A prototype for language-conditioned skill selection.
- [Code as Policies: Language Model Programs for Embodied Control](https://arxiv.org/abs/2209.07753) - Generates robot policy code that calls perception and control APIs.
- [ProgPrompt: Generating Situated Robot Task Plans using Large Language Models](https://arxiv.org/abs/2209.11302) - Represents task plans as program-like executable structures.
- [ROS-LLM: A ROS framework for embodied AI with task feedback and structured reasoning](https://arxiv.org/abs/2406.19741) - Connects LLM agents to ROS actions and services with multiple behavior modes.
- [VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models](https://voxposer.github.io/) - Composes 3D value maps and motion planning as robot tool use.
- [RAI: Robotic AI Agent](https://github.com/RobotecAI/rai) - A ROS2 physical AI agentic framework.

## Long-Horizon Manipulation

**Why this matters for Agentic Robotics:** long-horizon tasks expose the need for memory, progress tracking, error correction, and hierarchical control.

- [CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks](https://arxiv.org/abs/2112.03227) - A core benchmark for long-horizon language-conditioned manipulation.
- [Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware](https://arxiv.org/abs/2304.13705) - Introduces action chunking as a practical long-horizon control strategy.
- [Diffusion Policy: Visuomotor Policy Learning via Action Diffusion](https://arxiv.org/abs/2303.04137) - Uses action diffusion and receding-horizon control.
- [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) - A widely used open-source generalist VLA baseline.
- [pi0: A Vision-Language-Action Flow Model for General Robot Control](https://arxiv.org/abs/2410.24164) - Uses flow matching for general robot control.
- [pi0.5: a Vision-Language-Action Model with Open-World Generalization](https://arxiv.org/abs/2504.16054) - Targets open-world generalization in home environments.

## Embodied Navigation Agents

**Why this matters for Agentic Robotics:** navigation agents require grounded language understanding, spatial memory, lifelong exploration, and often multi-agent coordination.

- [Vision-and-Language Navigation: Interpreting visually-grounded navigation instructions in real environments](https://openaccess.thecvf.com/content_cvpr_2018/papers/Anderson_Vision-and-Language_Navigation_Interpreting_CVPR_2018_paper.pdf) - The classic R2R starting point for vision-and-language navigation.
- [Vision-Language Navigation with Embodied Intelligence](https://arxiv.org/html/2402.14304v1) - A system-level survey of VLN with embodied intelligence.
- [LM-Nav: Robotic Navigation with Large Pre-Trained Models of Language, Vision, and Action](https://arxiv.org/abs/2207.04429) - Combines LLM landmark parsing, VLM grounding, and navigation policy execution.
- [GOAT-Bench: A Benchmark for Multi-Modal Lifelong Navigation](https://arxiv.org/abs/2404.06609) - Evaluates multi-modal, lifelong, open-vocabulary navigation.
- [Uni-NaVid](https://pku-epic.github.io/Uni-NaVid/) - A video-based VLA navigation model for multiple embodied navigation tasks.
- [Co-NavGPT: Multi-Robot Cooperative Visual Semantic Navigation using Large Language Models](https://arxiv.org/abs/2310.07937) - Studies cooperative visual semantic navigation with multiple robots.

## Human-Robot Interaction and Dialogue Agents

**Why this matters for Agentic Robotics:** agentic robots operate with people, so dialogue, human feedback, mixed initiative, and human modeling are part of the control loop.

- [Inner Monologue: Embodied Reasoning through Planning with Language Models](https://arxiv.org/abs/2207.05608) - Incorporates human feedback into embodied planning.
- [Understanding LLM-powered Human-Robot Interaction](https://arxiv.org/abs/2401.03217) - Studies design requirements for LLM-powered HRI.
- [Large Language Models as Zero-Shot Human Models for Human-Robot Interaction](https://arxiv.org/abs/2303.03548) - Uses LLMs as human models for social robot planning.
- [A Survey on Dialogue Management in Human-Robot Interaction](https://arxiv.org/abs/2307.10897) - Surveys dialogue management for HRI.
- [MICoBot: Mixed-Initiative Dialog for Human-Robot Collaborative Manipulation](https://arxiv.org/html/2508.05535v1) - Studies robots that actively request human help.
- [Conversational Language Models for Human-in-the-Loop Multi-Robot Coordination](https://arxiv.org/abs/2402.19166) - Uses conversational models for multi-robot coordination with human input.

## Safety, Governance, and Physical Risk

**Why this matters for Agentic Robotics:** once agents gain execution authority in the physical world, safety, governance, consent, and runtime constraints become core system requirements.

- [Safety Guardrails for LLM-Enabled Robots](https://arxiv.org/abs/2503.07885) - Proposes guardrails for physical LLM-enabled robots.
- [Vision-Language-Action Safety: Threats, Challenges, Evaluations, and Mechanisms](https://arxiv.org/abs/2604.23775) - A VLA safety survey suitable as a section anchor.
- [Harnessing Embodied Agents: Runtime Governance for Policy-Constrained Execution](https://arxiv.org/abs/2604.07833) - Treats runtime governance as a distinct execution layer.
- [EmbodiedGovBench: A Benchmark for Governance-Constrained Embodied Agents](https://arxiv.org/html/2604.11174v1) - Evaluates whether embodied systems follow governance constraints.
- [Consent Chain Degradation in Embodied Multi-Agent Systems](https://arxiv.org/html/2605.16300v1) - Studies consent, delegation, and physical irreversibility in embodied multi-agent systems.
- [RoboGuard](https://github.com/KumarRobotics/RoboGuard) - Project page for safety guardrails for LLM-enabled robots.

## Benchmarks, Simulators, and Datasets

**Why this matters for Agentic Robotics:** agentic benchmarks should test long-horizon execution, memory, failure handling, recovery, multi-robot coordination, and safety, not just imitation quality.

- [Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864) - Cross-embodiment robot trajectories at large scale.
- [LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning](https://arxiv.org/abs/2306.03310) - A lifelong robot manipulation benchmark.
- [CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks](https://arxiv.org/abs/2112.03227) - Long-horizon language-conditioned manipulation benchmark.
- [BridgeData V2: A Dataset for Robot Learning at Scale](https://arxiv.org/abs/2308.12952) - A large-scale manipulation dataset.
- [RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots](https://arxiv.org/abs/2406.02523) - High-fidelity home and kitchen simulation.
- [Habitat 3.0: A Co-Habitat for Humans, Avatars and Robots](https://arxiv.org/abs/2310.13724) - Simulation for human-robot collaboration.

## Open-Source Systems and Frameworks

**Why this matters for Agentic Robotics:** open systems make it possible to compare architectures, reproduce results, and build practical robot agents beyond isolated model demos.

- [OpenVLA](https://github.com/openvla/openvla) - Open-source VLA model, training, and fine-tuning code.
- [Octo: An Open-Source Generalist Robot Policy](https://arxiv.org/abs/2405.12213) - An open-source generalist policy trained on Open X-Embodiment.
- [RoboFlamingo: Vision-Language Foundation Models as Effective Robot Imitators](https://arxiv.org/abs/2311.01378) - An imitation framework based on open-source VLMs.
- [ROS-LLM: A ROS framework for embodied AI with task feedback and structured reasoning](https://arxiv.org/abs/2406.19741) - ROS plus LLM agents, feedback, and behavior modes.
- [RAI](https://github.com/RobotecAI/rai) - A ROS2 physical AI agentic framework.
- [Open X-Embodiment](https://github.com/google-deepmind/open_x_embodiment) - Infrastructure for standardized robot learning data.

## Industrial Signals and Technical Reports

**Why this matters for Agentic Robotics:** industry reports and product signals reveal which agentic robot capabilities are moving toward deployment, even when full systems are not open-sourced.

- [Gemini Robotics: Bringing AI into the Physical World](https://arxiv.org/abs/2503.20020) - Google DeepMind's VLA and embodied reasoning technical report.
- [Gemini Robotics 1.5](https://arxiv.org/abs/2510.03342) - An industrial signal for physical agents, embodied reasoning, and motion transfer.
- [pi0: A Vision-Language-Action Flow Model for General Robot Control](https://arxiv.org/abs/2410.24164) - Physical Intelligence's generalist robot policy.
- [pi0.5: a Vision-Language-Action Model with Open-World Generalization](https://arxiv.org/abs/2504.16054) - Targets open-world home task generalization.
- [Hi Robot](https://www.pi.website/research/hirobot) - A hierarchical robot system with high-level VLM reasoning and low-level VLA control.
- [GR00T N1: An Open Foundation Model for Generalist Humanoid Robots](https://arxiv.org/abs/2503.14734) - NVIDIA's humanoid robot foundation model.

## Contributing

Contributions are welcome. To keep the list focused, please prefer entries that make a clear contribution to one of these agentic robotics capabilities:

- embodied memory
- planning and reasoning
- world modeling or world-action modeling
- verification and self-evaluation
- failure detection and recovery
- skill calling, tool use, or robot APIs
- long-horizon manipulation
- embodied navigation
- human-robot interaction
- safety, governance, or physical risk
- benchmarks that evaluate agentic behavior

For each new entry, include a short note explaining why it matters for agentic robotics.
