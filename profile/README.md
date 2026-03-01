# Emergent State Machine (ESM)

Emergent State Machine (ESM) is a formal, turn-based control architecture pattern for systems where probabilistic interpretation must coexist with deterministic authority.

ESM separates:

- Descriptive state representation  
- Deterministic, versioned policy authority  
- Controlled mutation at the decision boundary  
- Optional schema-constrained generative instrumentation  

The result is a system that is more auditable, replayable, and governable as AI components evolve.

---

## Repository

### 📘 esm-spec
The normative specification of the ESM pattern (execution model, layer separation, and turn structure).

---

## Relationship to Controlled Mutation Layer (CML)

CML is a specification + SDK family for instrumenting mutation events at the decision boundary.

ESM is the broader control architecture pattern that can incorporate CML.

ESM and CML can be adopted independently, but they are designed to work well together.
