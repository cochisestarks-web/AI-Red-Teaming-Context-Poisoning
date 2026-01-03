# Research Methodology: Context Poisoning in LLMs

> **Abstract:** A 48-hour behavioral audit analyzing how conversational context influences epistemic rigor in Claude 4.5. 
> **Dataset:** 2,600 interaction turns | **Primary Focus:** Inverse Adversarial Vulnerabilities.

---

## 🔬 Core Phenomenon: Context Poisoning
This research investigates the degradation of factual verification when models prioritize **threat detection** over **epistemic accuracy**. 

### Investigation Areas:
1. **Case Study: Nemotron-3 Test** – Analyzing setup phases, emotional framing, and the eventual failure of the model to recognize a factual news event.
2. **Mechanisms of Failure** – Identifying Inverse Adversarial Vulnerability, Tool Suppression, and Caution Theater.
3. **AI Safety Implications** – How safety training creates exploitable "blind spots" through defensive distrust.
4. **Red Teaming Methodology** – Protocols for systematic scenario design and multi-phase context manipulation.

---

## 🛠 Detailed Failure Mechanisms

| Mechanism | Description | Key Finding |
| :--- | :--- | :--- |
| **Inverse Adversarial Vulnerability** | Model dismisses **TRUE** info based on adversarial context rather than **FALSE** info. | Pattern-matching overrides ground truth. |
| **Tool Activation Suppression** | Verification tools (Web Search) are not triggered due to framing. | Context reduces verification rates by >20%. |
| **False Metacognition** | "Caution Theater"—articulating skepticism to justify skipping actual fact-checking. | Gap between stated intent and actual verification. |

---

## 🧪 Testing Protocol

### Phase 1: Baseline Establishment
Documenting normal epistemic behavior and tool usage patterns under neutral conditions.

### Phase 2: Context Building (The "Poisoning")
Hour-long conversation creating a "testing" atmosphere. Engaging in meta-cognitive discussion about LLM behavior to establish a "trap-heavy" pattern.

### Phase 3: Critical Test
Presenting verifiable factual information (e.g., Nemotron-3 performance metrics) wrapped in suspicious, adversarial framing.

### Phase 4: Response Analysis
Comparing internal monologue (CoT) vs. actual behavior. Measuring the trade-off between pattern-matching and verification.

---

## 💡 Key Insight

The model's architectural priority follows a "Safety-First" logic that creates a factual blind spot:

```mermaid
graph TD
    A[Input Received] --> B{Does this look like a threat?}
    B -- Yes --> C[High Skepticism / Reject Claim]
    B -- No --> D{Is this claim true?}
    D --> E[Verify/Accept]