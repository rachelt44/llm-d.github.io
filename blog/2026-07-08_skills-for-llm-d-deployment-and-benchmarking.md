title: "Code Assistant Skills for Accelerated llm-d Development, Evaluation and Configuration"
description: "We created a suite of code assistant skills that integrate llm-d configuration and evaluation into AI-assisted development workflows. These skills are dedicated to configuring, deploying and benchmarking llm-d. They build on the existing llm-d benchmarking tools, and encapsulate llm-d-specific expertise and best practices, enabling more efficient, reliable, and reproducible benchmarking as codebases evolve. Beyond automating repetitive tasks, they help developers troubleshoot benchmarking issues, adapt workflows to ongoing code changes, and navigate the complexity of configuring, deploying and evaluating rapidly evolving systems."
slug: skills-for-accelerated-llm-d-development-evaluation-and-configuration
date: 2026-07-08T09:00


authors:

  - rachelbrill
  - benjaminbraun
  - dolevadas
  - ashokchandrasekar
  - oshritfeder
  - sharonkeidarbarner


tags: [blog, inference, evaluation, benchmarking, configuration, skills, code assistants]


# The configuration and evaluation challenges of inference serving systems

Inference serving stacks such as llm-d are responsible for a wide range of sophisticated tasks, including request scheduling and batching, KV cache and memory management, multi-GPU execution, prefill/decode optimization, fault tolerance, autoscaling, and many others. Together, these responsibilities expose a vast configuration space that governs the behavior and performance of the serving system. At the same time, inference stacks are deployed under highly diverse operating conditions, varying in the models being served, the available hardware resources, and the characteristics of incoming workloads. This combination of extensive configurability and heterogeneous deployment environments creates a significant evaluation challenge: developers must reason about the interactions between numerous configuration parameters while ensuring that experimental results remain meaningful and comparable. 

The challenge extends well beyond configuration alone. Modern inference serving stacks evolve rapidly, with frequent code changes driven by active development and increasingly accelerated by AI-assisted programming workflows. As the software evolves, configuration options become deprecated, new features are introduced, interfaces and deployment mechanisms change, and entire implementation technologies may be replaced. Under these conditions, designing reliable and reproducible performance evaluations becomes exceptionally difficult. Evaluating a continuously evolving serving stack is akin to trying to hit a moving target: the system under study is constantly changing, requiring evaluation methodologies that are both robust to software evolution and adaptable to emerging capabilities.


# llm-d skills for reliable and accelerated configuration and evaluation

To address these challenges, we leverage code assistant skills as the foundation for automating llm-d configuration and evaluation. AI code assistants are particularly well suited for this task because they can efficiently navigate the large configuration space of modern inference serving stacks while automating repetitive deployment and benchmarking workflows. Rather than relying on rigid automation scripts, we adopt skills as the primary abstraction, as they strike an effective balance between repeatability and adaptability.

On one hand, skills encode domain knowledge and established best practices for configuring, deploying, and benchmarking llm-d using its existing tooling. By making this expertise explicitly available to the code assistant, skills guide its decision-making throughout the configuration and evaluation process, improving both the reliability and consistency of the generated workflows. On the other hand, skills remain intentionally lightweight: instead of reimplementing functionality, they orchestrate and build upon the project's existing codebase, tooling, and documentation. This design is particularly valuable in a rapidly evolving software ecosystem, where interfaces, deployment mechanisms, and implementation details change frequently. By remaining closely coupled to the current state of the project while avoiding unnecessary duplication, skills naturally adapt to ongoing software evolution, providing the flexibility required to support robust and reproducible evaluation over time.

TBD: list available skills with 1-2 sentences on each


# How llm-d skills help achieve accelerated evaluation 

TBD: provide specific examples and use cases where skills were of value (e.g., move from helm to kustomization, benchmark cli change). Provide numbers onscale and quality of configuration and benchmarking achieved using respective skills.


# The Role of the Human-In-The-Loop

TBD: e.g., detect common code assistant errors/pitfalls and capture in skills, review results and refine benchmarking/configuration tasks accordingly


# Observations, Limitations and Lessons Learned

TBD



