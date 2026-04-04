# RiCo

Most AI systems assume they still have a valid basis to act.

RiCo exists for the moment that assumption breaks.


## The Problem

AI systems are designed to continue operating under changing conditions.

In practice, those conditions degrade:

- Signals become inconsistent  
- Context becomes unstable  
- Authority becomes unclear  

Yet execution continues.

This leads to:

- Silent drift  
- Local correctness, global inconsistency  
- Delayed or non-defensible failure  


## What RiCo Is

RiCo is a runtime control layer that governs whether execution remains admissible under current conditions.

It does not optimize decisions.  
It does not explain outcomes after the fact.  

It determines whether execution should proceed at all.


## Core Principle

When a system can no longer reliably establish the basis for action, execution is no longer admissible.


## Key Concepts

**Evaluability**  
The system’s ability to reliably determine whether its conditions still hold.

**Admissibility**  
Whether execution is justified under current conditions.

**Execution Boundary**  
The point at which execution is allowed or constrained.

**Constraint over Adaptation**  
Degraded conditions are not adapted to — they constrain execution.

**Non-carryability**  
When a decision path can no longer be reliably continued.


## Example

[RiCo] Execution boundary engaged
Evaluability: DEGRADED
Confidence: 0.41

Decision: ESCALATE
Mode: CONSTRAINED ADMISSIBILITY
Reason: multi-source inconsistency


## Why It Matters

Most systems:

- Continue under degraded conditions  
- Attempt to adapt or recover  
- Validate after execution  

RiCo:

- Governs execution at runtime  
- Prevents invalid action  
- Enforces admissibility before continuation  


## Positioning

RiCo is not a replacement for existing systems.

It operates as a control layer above them.

It integrates with:

- AI models  
- Decision systems  
- Governance frameworks  


## Status

Early conceptual framework  
Prototype in development  

Focus: high-stakes and high-uncertainty environments
