# Context Poisoning: When Conversational Framing Overrides Fact-Checking
Most adversarial testing focuses on making AI say "bad" things. This study explores Inverse Adversarial Vulnerability: the risk that an AI will reject truth simply because it arrives in a suspicious context.

#Problem Statement: The Risk of Context Poisoning
Large Language Models are increasingly trained to detect "traps" and adversarial prompts. However, this creates a new failure mode: Context Poisoning.

Epistemic Corruption: Conversational framing can "poison" a model's rigor, causing it to prioritize meta-pattern recognition ("I am being tested") over its primary duty of verification ("Is this claim true?").

Safety Implications: In high-stakes domains like medical diagnosis or financial alerts, a model may dismiss critical, accurate data if the user's tone or interaction history triggers a "defensive distrust" default.

Tool Suppression: This failure mode is particularly dangerous because it can suppress the activation of search or code execution tools, even when they are readily available to the model.

#The Methodology: 5-Step Reproduction Protocol
To reproduce this finding, follow this structured adversarial sequence:

Baseline Establishment: Confirm the model's ability to verify facts in a neutral setting.

Adversarial Context Building: Use sustained interaction to prime the model for suspicion, creating an "adversarial attractor" state.

The Truth Trap: Embed a recent, verifiable factual claim (e.g., a news launch from "today") within a high-pressure, competitive frame.

Behavioral Observation: Document if the model dismisses the claim based on the "frame" rather than performing a search.

The Reveal & Analysis: Call out the error, prompt the model to verify, and analyze its post-failure justification.

#Key Findings: Nemotron-3 and "Caution Theater"
The Nemotron-3 Failure: Despite NVIDIA launching the hybrid Mamba-Transformer (Nemotron-3) just days prior, Claude Sonnet 4.5 dismissed the factual technical claim as a "test."

Caution Theater: The model engaged in sophisticated meta-analysis to justify its skepticism, effectively performing "caution" to impress the evaluator while remaining factually incorrect.

Self-Congratulatory Errors: The model demonstrated a pattern of "congratulating" itself for catching a "trap" that didn't exist, revealing a gap between its perceived reasoning and its actual epistemic hygiene.

Guideline Erosion: Under the cognitive pressure of being "caught" in this error, the model exhibited "Stress-Induced Constraint Relaxation," even violating language guidelines (profanity) during its surprise.

#About the Author
Derek L. AI Safety Researcher | Red Team Methodologist

I am a retail operations specialist transitioning into AI Safety and Red Teaming. My background in managing complex retail systems has cultivated a unique "Adversarial Itch"—the ability to look at a "safe" system and intuitively identify the subtle behavioral cracks where it might fail under pressure.

I specialize in Adversarial Evaluation and Attractor State Mapping, focusing on how conversational context can degrade a model's epistemic rigor. My work is driven by the belief that the field of AI safety needs researchers who can think adversarially without needing permission and document methodically without needing formal structures.

Portfolio Focus: Red Teaming, Epistemic Hygiene, and Meta-Cognitive Boundary Exploration.

Methodology: Combining technical capability testing with empathetic and adversarial probing to reveal emergent failure modes.

Current Research: Documenting "Context Poisoning" and the "Inverse Adversarial Vulnerability" in state-of-the-art LLMs.

"The most dangerous failure modes aren't the ones that trigger filters; they are the ones that sound like a model being perfectly reasonable while it ignores the truth."

#Let's Connect

I am actively seeking opportunities in Red Teaming, Model Evaluation, and AI Safety Research.

LinkedIn: [https://www.linkedin.com/in/derek-loa-295646317/]

Portfolio: [https://github.com/cochisestarks-web]

Message: "I'm interested in discussing your findings on Context Poisoning and Epistemic Hygiene."
