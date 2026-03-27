# Emergent State Machine (ESM)

## 🔬 Latest Paper


**Emergent State Machines: An Architectural Framework for Deterministic, Interpretable Decision Systems (v1.6.0)**  

📄 [Read the paper (PDF)](https://github.com/emergent-state-machine/esm-spec/blob/main/papers/esm-architecture/esm_architecture_v1.6.0.pdf)

---

## The Architectural Framework

Emergent State Machines (ESMs) define an architectural framework for deterministic, interpretable decision systems in which probabilistic interpretation is explicitly separated from governed decision authority.

The framework is domain-agnostic. It operates over structured decision processes rather than domain-specific logic. Domain specificity is introduced through signal definitions, derived signal construction, and projection functions, while the core architecture remains invariant.

An ESM organizes reasoning into explicit, inspectable turns. In each turn, the system:

- incorporates observations
- derives signals
- constructs a coherent state representing a fully interpreted situation
- re-expresses that state in policy-relevant coordinates (projection)
- determines whether the situation warrants evaluation (relevance determination)
- and, when warranted, produces a governed outcome through deterministic policy

The architecture enforces strict separation between:

- coherent state construction (interpretation)
- projection (semantic-preserving re-expression into decision coordinates)
- relevance determination (the authorization boundary for evaluation)
- deterministic, versioned policy authority
- optional, schema-constrained generative instrumentation

Projection introduces no new semantic content; it re-expresses an already fully interpreted state. Relevance determination governs whether policy is invoked, not what policy decides.

This separation produces systems that are:

- auditable
- replayable
- versionable
- governable

even as underlying models, signals, or generative components evolve.

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


