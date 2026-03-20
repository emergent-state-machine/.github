# Emergent State Machine (ESM)

## 🔬 Latest Paper


**Emergent State Machines: A Deterministic Control Framework for Interpretable Situational Reasoning (v1.3.0)**  

📄 [Read the paper (PDF)](https://github.com/emergent-state-machine/esm-spec/blob/main/papers/esm-architecture/esm_architecture_v1.3.0.pdf)

---

## The Architecture

Emergent State Machine (ESM) is a formal, turn-based control architecture pattern for systems where probabilistic interpretation must coexist with deterministic authority.

ESM separates:

- Descriptive state representation  
- Deterministic, versioned policy authority  
- Controlled mutation at the decision boundary  
- Optional schema-constrained generative instrumentation  

The result is a system that is more auditable, replayable, and governable as AI components evolve.

--- 

## Repository

### 📘 [esm-spec →](https://github.com/emergent-state-machine/esm-spec)

Normative specification and formal definitions. 

---

## Relationship to Controlled Mutation Layer (CML)

The Emergent State Machine (ESM) is the architectural pattern.

Reference implementations and mutation-boundary instrumentation are provided by the Controlled Mutation Layer (CML):

🔧 CML Organization
https://github.com/controlled-mutation-layer

🐍 Python Reference SDK
https://github.com/controlled-mutation-layer/sdk-python

ESM defines how state evolves.
CML instruments the mutation boundary.

ESM and CML can be adopted independently, but they are designed to work well together.


