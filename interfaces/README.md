# Interfaces

This directory defines the implementation-neutral interfaces used by RiCo (Runtime Integrity Control).

RiCo is designed as a governance layer rather than an execution engine. These interface specifications describe how external systems exchange observations, execution requests, governance decisions, and runtime evidence with the Runtime Execution Boundary (REB).

The goal is interoperability without prescribing internal implementations.

## Principles

- Implementation-neutral
- Runtime-oriented
- Technology agnostic
- Traceable
- Portable
- Governable

## Interface Specifications

| Document | Purpose |
|----------|---------|
| `OBSERVATION_CONTRACT.md` | Defines the structure and expectations for runtime observation inputs. |
| `EXECUTION_CONTRACT.md` | Defines execution requests presented to the Runtime Execution Boundary. |
| `GOVERNANCE_RECEIPT.md` | Defines the portable governance decision artifact produced by RiCo. |
| `REB_INTERFACE.md` | Defines the Runtime Execution Boundary interface between execution systems and governance. |

## Architectural Goal

The Runtime Execution Boundary provides a stable governance interface through which observations, runtime assessments, admissibility decisions, and governance receipts remain independent of any particular AI model, execution engine, or infrastructure implementation.

---

Humans First. Continuity Always. Architecture Must Survive.
