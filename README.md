# RiCo

Most AI systems assume they still have a valid basis to act.

RiCo exists for the moment that assumption breaks.

---

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

---

## What RiCo Is

RiCo is a runtime control layer that governs whether execution remains admissible under current conditions.

It does not optimize decisions.  
It does not explain outcomes after the fact.  

It determines whether execution should proceed at all.

---

## Core Principle

When a system can no longer reliably establish the basis for action, execution is no longer admissible.

RiCo treats loss of evaluability as a constraint on execution — not a condition to adapt through.

---

## Execution Flow

INPUT → VALIDATE → EVALUATE → DECIDE → EXECUTE / CONSTRAIN

1. INPUT  
   Action request enters the system  

2. VALIDATE  
   Authority and policy checks  

3. EVALUATE  
   Are conditions still reliable? (Evaluability)

4. DECIDE  
   Is execution admissible under current conditions?

5. OUTCOME  
   - EXECUTE → proceed normally  
   - CONSTRAIN → escalate, defer, or terminate  

---

## Decision Modes

RiCo does not treat execution as binary (allow / deny).

It operates across modes:

- **Admissible** → execution proceeds  
- **Constrained Admissibility** → execution limited or escalated  
- **Non-admissible** → execution does not proceed  

Mode is determined by evaluability and confidence thresholds.

RiCo does not manage outcomes — it governs whether outcomes are allowed to be produced at all.

---

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

---

## Example

[RiCo] Execution boundary engaged
Evaluability: DEGRADED
Confidence: 0.41

Decision: ESCALATE
Mode: CONSTRAINED ADMISSIBILITY
Reason: multi-source inconsistency

---

## Why It Matters

Most systems:

- Continue under degraded conditions  
- Attempt to adapt or recover  
- Validate after execution  

RiCo:

- Governs execution at runtime  
- Prevents invalid action  
- Enforces admissibility before continuation  

---

## Positioning

RiCo is not a replacement for existing systems.

It operates as a control layer above them.

It integrates with:

- AI models  
- Decision systems  
- Governance frameworks  

---

## Status

Early conceptual framework  
Prototype in development  

Focus: high-stakes and high-uncertainty environments

Focus: high-stakes and high-uncertainty environments
