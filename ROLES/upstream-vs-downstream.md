# Upstream vs Downstream

This document defines the upstream / downstream distinction used throughout Constraint Architecture.

This distinction is structural, not organizational.
It is determined by **timing relative to execution**, not by seniority, prestige, or proximity to systems.

---

## The Axis That Matters

There is only one axis:

> **Can this work still change whether an action executes?**

If yes, it is upstream.
If no, it is downstream.

---

## Upstream

**Upstream work occurs before execution.**

Upstream roles:

* define admissibility
* set constraints
* commit authority
* eliminate ambiguity

Upstream work can:

* prevent execution
* allow execution
* remove invalid actions entirely

Examples:

* Constraint Architect
* execution admissibility design (512-class kernels)
* contract and policy definition converted into constraints
* execution boundary mapping

Once execution begins, upstream authority ends.

---

## Downstream

**Downstream work occurs after execution.**

Downstream roles:

* observe
* record
* interpret
* analyze
* explain

Downstream work can:

* reconstruct events
* assign responsibility
* support audit and learning

Downstream work cannot:

* prevent the action
* reverse the outcome
* deny execution

Examples:

* CVS systems integration
* CVS forensics and replay
* audit and compliance reporting
* incident analysis

---

## Common Category Errors

Mistakes occur when:

* monitoring is treated as control
* audit is mistaken for prevention
* interpretation is confused with authority
* escalation is assumed to arrive in time

These errors collapse upstream and downstream into a single imagined layer.

Constraint Architecture exists to prevent that collapse.

---

## Why This Distinction Exists

For most of human history, execution was slow enough that upstream and downstream appeared merged.

Human intervention could still arrive in time.

At machine speed, they separate.

Once execution outruns humans, authority must move upstream — or vanish.

---

## Final Note

Upstream and downstream are not hierarchies.

They are positions relative to irreversibility.

If you cannot still stop the action, you are downstream.
