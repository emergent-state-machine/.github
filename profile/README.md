# Emergent State Machine (ESM)

## 🔬 Latest Paper


**Emergent State Machines: A Deterministic Control Framework for Interpretable Situational Reasoning (v1.3.0)**  

📄 [Read the paper (PDF)](https://github.com/emergent-state-machine/esm-spec/blob/main/papers/esm-architecture/esm_architecture_v1.3.0.pdf)

---

## The Architecture

## The Framework

Emergent State Machines (ESMs) define a formal, turn-based control framework for systems in which probabilistic interpretation must coexist with deterministic authority.

The framework is domain-agnostic: it operates over structured decision processes rather than domain-specific logic. Domain specificity is introduced through signal definitions, derived signal construction, and projection primitives, while the core control structure remains unchanged.

An ESM organizes reasoning into explicit, inspectable turns, each of which transforms observations into signals, constructs an interpretable state representation, evaluates relevance, and, when warranted, maps deterministically to an action or other outcome.

ESM enforces structural separation between:

- descriptive state representation
- projection into policy-relevant coordinates
- relevance gating (decision eligibility)
- deterministic, versioned policy authority
- optional schema-constrained generative instrumentation

This separation produces systems that are auditable, replayable, and governable, even as underlying models, signals, or generative components evolve.

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


