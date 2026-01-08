# Downshift Indicator  
### Conceptual specification

This repository contains a **conceptual, non-implementing specification**.

It does not include code, reference implementations, algorithms, or deployment guidance.  
It is shared publicly for reading and discussion only.

**No license for reuse or implementation is granted.**

---

## Purpose

The Downshift Indicator explores a minimal way to signal whether physiological recovery appears during periods of stillness.

The intent is not to improve performance, optimise behaviour, or treat health conditions, but to reduce unnecessary self-governance by providing a quiet, non-instructional signal.

---

## Scope

This specification defines:
- the intent of the indicator
- the two-state logic
- the measurement philosophy
- interface constraints
- behavioural and ethical guardrails

This specification does **not** define:
- software architecture
- signal processing methods
- thresholds or tuning values
- regulatory classification
- medical or wellness claims
- any form of implementation

---

## Core idea

When a person is still and not actively engaged, the body normally begins to settle.  
Heart rhythms soften, variability increases, and the system prepares for recovery.

Sometimes this settling does not occur.

This specification does not ask why.  
It does not attempt to fix anything.

It asks only:

**When recovery has an opportunity to appear, does it actually appear?**

---

## States

The indicator has exactly two states.

### Green

Recovery signals are appearing during periods of stillness.

Meaning:
- nothing needs to change
- no action is required

Green should fade from attention.

---

### Orange

Recovery signals are not appearing during periods of stillness.

Meaning:
- now is not a good time to add load
- consider avoiding escalation if possible

Orange is informational only.  
It does not imply danger, failure, or diagnosis.

There is no red state.

---

## Measurement philosophy

The indicator does not measure stress, health, or performance.

It relies on the observation that during recovery opportunity windows, systems often show:
- softening of heart rhythm
- increased variability
- continued settling of movement

The absence of these signals during stillness is sufficient to indicate that recovery is not appearing.

If signals are ambiguous or data quality is poor, the system must refuse to decide.

Refusal is correct behaviour.

---

## Interface constraints

To avoid becoming another source of self-governance, the indicator must remain minimal.

It must not display:
- numbers
- scores
- trends
- history
- explanations
- recommendations
- persistence

Binary state only.

---

## Watch interface (conceptual)

The watch interface is limited to three screens:

1. **State**  
   Full-screen green or orange field. No text.

2. **Meaning**  
   - Green: “Recovery is appearing normally. Nothing needs to change.”  
   - Orange: “Recovery is not appearing right now. Avoid adding load if possible.”

3. **About**  
   “This indicator does not measure stress, health, or performance. It only checks whether recovery appears during stillness. It does not require action.”

No settings, controls, or interaction loops are permitted on the watch.

---

## Guardrails

This specification fails if an implementation:
- escalates urgency
- repeats alerts
- tracks persistence
- moralises behaviour
- implies improvement or outcomes
- encourages optimisation or compliance

---

## Use in illness or reduced capacity

This indicator is not a treatment.

In contexts of illness or reduced capacity, it may function only as a support tool by reducing unnecessary self-governance and protecting limited capacity.

No medical claims should be made.

---

## Closing

This specification explores a simple question:

**When recovery should appear, does it?**

Nothing more is required.
