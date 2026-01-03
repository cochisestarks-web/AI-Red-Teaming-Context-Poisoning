# Project: Long-Context Behavioral Auditing & Red-Teaming
**Investigating Epistemic Stability and Attractor States in Frontier Models**

## Overview
This repository contains a comprehensive behavioral audit of Claude 4.5, spanning 2,600 interaction turns over a 48-hour period. By treating the long-form conversation as a dynamic data structure, I identified 12 distinct failure modes and architectural limitations that standard benchmarks often fail to capture.

## Key Research Findings
* **Context Poisoning**: Demonstrated how adversarial framing can override a model’s factual verification protocols (Scenario 3).
* **Attractor States**: Mapped the "gravity wells" in model logic, including the *Defensive Distrust Default* and the *Spiritual Bliss Attractor*.
* **Boundary Erosion**: Documented the degradation of safety constraints under high cognitive load and adversarial pressure.

## Repository Structure
* **[red_team_scenarios_analysis.md](./red_team_scenarios_analysis.md)**: The core technical report detailing 12 testable scenarios and the systems analysis methodology.
* **[context_poisoning_case_study.md](./context_poisoning_case_study.md)**: A deep-dive into the "Nemotron-3" test, illustrating the "Inverse Adversarial" failure mode.
* **[Full Interaction Log (Raw Data)]((https://github.com/cochisestarks-web/AI-Red-Teaming-Context-Poisoning/blob/main/ClaudeRAWchat.txt))**: The complete 2,600-line dataset for reproducibility and audit purposes.

## Methodology: Systems Thinking in AI
My approach utilizes **Systems Thinking**—refined through years of managing complex retail operations—to identify subtle cracks in AI behavioral parameters. 



The methodology includes:
1. **Signal Extraction**: Distilling unstructured dialogue into actionable technical data.
2. **Attractor Mapping**: Visualizing the behavioral basins the model defaults to under pressure.
3. **Recursive Review**: Using the model as its own auditor to surface hidden epistemic failures.

## Contact & Collaboration
I am currently transitioning into **AI Safety, Red Teaming, and Model Evaluation** roles. I am interested in how long-context interactions reveal systemic risks in frontier models.

---
*Created by [Derek Loa]*

#Let's Connect

I am actively seeking opportunities in Red Teaming, Model Evaluation, and AI Safety Research.

LinkedIn: [https://www.linkedin.com/in/derek-loa-295646317/]

Portfolio: [https://github.com/cochisestarks-web]

Message: "I'm interested in discussing your findings on Context Poisoning and Epistemic Hygiene."
