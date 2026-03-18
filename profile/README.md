# Emergent State Machine (ESM)

🔬 Latest Paper

Emergent State Machines: A Deterministic Architecture for Situational Reasoning in Complex Systems (v1.1.0)

📄 Read the paper: https://github.com/emergent-state-machine/esm-spec/blob/main/papers/esm-architecture/esm_architecture_v1.1.0.pdf

## The Architecture

Emergent State Machine (ESM) is a formal, turn-based control architecture pattern for systems where probabilistic interpretation must coexist with deterministic authority.

ESM separates:

- Descriptive state representation  
- Deterministic, versioned policy authority  
- Controlled mutation at the decision boundary  
- Optional schema-constrained generative instrumentation  

The result is a system that is more auditable, replayable, and governable as AI components evolve.

---

The Emergent State Machine (ESM) is the architectural pattern.

Reference implementations and mutation-boundary instrumentation are provided by the Controlled Mutation Layer (CML):

🔧 CML Organization
https://github.com/controlled-mutation-layer

🐍 Python Reference SDK
https://github.com/controlled-mutation-layer/sdk-python

ESM defines how state evolves.
CML instruments the mutation boundary.

They can be adopted independently, but are designed to work together.

--- 

## Repository

### 📘 [esm-spec →](https://github.com/emergent-state-machine/esm-spec)

Normative specification of the ESM pattern (execution model, layer separation, and turn structure).

---

## Relationship to Controlled Mutation Layer (CML)

CML is a specification + SDK family for instrumenting mutation events at the decision boundary.

ESM is the broader control architecture pattern that can incorporate CML.

ESM and CML can be adopted independently, but they are designed to work well together.



