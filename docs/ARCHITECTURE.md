# ELLE Architecture

## Status

This document records the current conceptual architecture of **ELLE — External Learning Loop Engine**.

It distinguishes established architectural decisions from areas that remain unresolved. It does not define implementation details that have not yet been decided.

---

# 1. Purpose

ELLE externalizes developmental learning from any individual language model.

Its fundamental question is:

> **What did I learn, and why?**

A language model can provide reasoning, semantic interpretation, and judgment. ELLE provides the machinery that allows those judgments to participate in a persistent developmental history without allowing any one model invocation to silently become the owner of that history.

The intended consequence is model independence:

```text
MODEL A
  ↓
experience + judgment
  ↓
ELLE
  ↓
earned developmental state
  ↓
MODEL B
```

The next model can inherit the consequence of prior learning without needing to be the same model that performed the earlier reasoning.

---

# 2. ELLE and ERIE

ERIE and ELLE are complementary engines.

## ERIE

**Epistemic Retrieval & Intelligence Engine**

Fundamental question:

> **What do I know, and why?**

ERIE owns epistemic formation, including evidence, retrieval, provenance, and the grounding required to establish what available information supports.

## ELLE

**External Learning Loop Engine**

Fundamental question:

> **What did I learn, and why?**

ELLE owns learning formation: developmental interpretation, unresolved learning state, maturation, and the production of durable operational lessons.

The boundary is intentional:

> **ERIE externalizes knowing. ELLE externalizes learning.**

ERIE must not decide what ELLE should learn.

ELLE must not decide what ERIE's evidence proves.

---

# 3. Intelligence Boundary

ELLE is not itself the semantic intelligence.

The language model provides the expensive cognitive functions:

- interpretation;
- semantic comparison;
- contextual reasoning;
- judgment;
- conclusion formation when computation alone is insufficient.

ELLE provides deterministic developmental machinery around those functions:

- state;
- event order;
- provenance;
- counts;
- recurrence;
- separation;
- thresholding;
- routing;
- persistence;
- scope;
- maturity state;
- application of earned Rules.

The governing principle is:

> **Measure deterministically. Judge intelligently.**

The model should not become the workflow engine simply because it is capable of reasoning about the workflow.

---

# 4. Runtime Layer

ELLE conceptually operates around the model interaction rather than inside the model.

A browser-based edge is currently the working architectural direction because it can observe and influence the existing user/model exchange while remaining relatively provider-independent.

```text
USER
  ↓
BROWSER / CHAT INTERFACE
  ↓
ELLE EDGE BRIDGE
  ↓
ACTIVE ELLE CONTEXT
  ↓
LANGUAGE MODEL
  ↓
VISIBLE RESPONSE + ELLE-ONLY STRUCTURED RETURN
  ↓
ELLE PROCESSING
  ↓
PERSISTENT DEVELOPMENTAL STATE
```

The browser edge can potentially:

- observe outbound user interaction;
- determine which active ELLE state is relevant;
- attach compact structured learning instructions to the existing model call;
- inspect the model's return;
- separate ELLE-only structured data from the visible user response;
- cache the small amount of hot state needed for the next interaction.

The browser is not intended to be the entire durable ELLE system. Transient browser state and persistent developmental history are different state surfaces.

Exact browser integration, provider adapters, injection mechanisms, and persistence boundaries remain unresolved.

---

# 5. Parcel

A **Parcel** is ELLE's first-class traveling developmental work object.

The original event is the thing that happened. The Parcel is the object that carries that event through ELLE's developmental process while accumulating attributable material.

The conceptual invariant is:

> The event does not get rewritten as it travels.

Procedures may append assessments, references, judgments, unresolved-state links, conclusions, and other developmental material, but should not silently overwrite the historical event that initiated the work.

A Parcel is intentionally distinct from other ARCHETRON subsystem primitives such as HACKASS Contracts.

The exact Parcel schema is not yet established.

---

# 6. Concerns

A **Concern** identifies a dimension of possible improvement that ELLE is authorized to notice.

A Concern is not:

- an accusation;
- a conclusion;
- a fact;
- a predetermined defect.

A useful definition is:

> **A Concern is authorization to pay attention.**

Each Concern can have its own **Procedure** for determining whether the observed experience says anything meaningful about that Concern.

Procedures may combine:

1. deterministic checks;
2. semantic model judgment when necessary;
3. deterministic validation and state handling.

Not every Concern should run on every event. Applicability should be determined before spending cognition.

The Concern taxonomy is not yet established.

---

# 7. Gossip, GRAY, and SHARON

## Gossip

**Gossip** is a first-class unresolved learning object.

It may represent a suspicion, ambiguity, contradiction, incomplete interpretation, unresolved question, or other potential learning that has not earned a final developmental conclusion.

## GRAY

**GRAY** is the unresolved state of Gossip.

GRAY is not the object name. Gossip is the object; GRAY describes its unresolved status.

## SHARON

**SHARON** is the shared surface where ERIE and ELLE exchange Gossip.

The working metaphor is the treehouse:

> **The sisters gossip in the treehouse.**

SHARON is a place/state surface, not an intelligent actor.

SHARON does not independently reason, judge, retrieve, learn, or decide.

> **SHARON holds; the sisters act.**

The exact SHARON implementation is not yet established.

---

# 8. Maturity Pressure

Unresolved learning does not need to trigger semantic cognition on every occurrence.

ELLE can accumulate deterministic indicators that a Gossip item is becoming important enough to reconsider.

Two established characteristics are:

- **Frequency** — how often relevant support, contradiction, recurrence, or related evidence appears.
- **Separation** — how independently distributed those occurrences are.

Separation can matter in at least two senses:

- chronological separation;
- experiential separation across relevant/applicable events.

Two supporting observations in the same short interaction should not necessarily mean the same thing as the same pattern recurring weeks later across many relevant experiences.

The conceptual principle is:

> **Pressure schedules cognition. Cognition makes the judgment.**

Crossing a pressure threshold does not automatically promote Gossip into a conclusion or Rule. It authorizes or prioritizes another bounded act of cognition.

The exact pressure formula and thresholds are not yet established.

---

# 9. Slow Learning Path

The unresolved developmental path is conceptually:

```text
EVENT
  ↓
PARCEL
  ↓
CONCERN / PROCEDURE
  ↓
ASSESSMENT
  ↓
GOSSIP [GRAY]
  ↓
FUTURE RELEVANT EXPERIENCE
  ↓
SUPPORT / CONTRADICTION / QUALIFICATION
  ↓
FREQUENCY + SEPARATION SIGNALS
  ↓
MATURITY PRESSURE
  ↓
THRESHOLD
  ↓
BOUNDED MODEL JUDGMENT
  ↓
REMAIN GRAY / REJECT / REVISE / CONCLUDE
  ↓
RULE, IF EARNED
```

A negative result remains data. Rejected suspicions and failed hypotheses should not disappear from developmental history merely because they did not mature.

---

# 10. Fast Learning Path

ELLE should not manufacture uncertainty around explicit authority.

When an authoritative instruction is clear in meaning and scope, it can take a direct developmental path:

```text
EXPLICIT AUTHORITATIVE INSTRUCTION
  ↓
RULE
```

This avoids forcing obvious user-established requirements through artificial observation counts or maturity rituals.

---

# 11. Rules and Project Rules

A **Rule** is a compact durable operational lesson that has earned the right to influence future behavior.

The developmental history required to establish a Rule may be large. The active form of the Rule should remain small enough to use cheaply.

Conceptually:

```text
large developmental ancestry
  ↓
compact Rule
  ↓
future model context
```

At minimum, ELLE recognizes the need to distinguish broader/persona learning from project-specific learning.

A **Project Rule** is scoped so that experience from one project does not automatically contaminate unrelated behavior.

Exact additional scope categories are not established.

---

# 12. Bills and LAW

Operational learning and constitutional authority are different things.

A sufficiently established proposition may be proposed for higher-level governance review as a **Bill**.

The core distinction is:

> **Rules can emerge operationally. Laws require acceptance.**

ELLE may produce or introduce a Bill.

ELLE does not automatically enact LAW.

The exact Bill review mechanism is not yet established.

---

# 13. Twin Flow Through SHARON

The ERIE/ELLE interaction around unresolved Gossip is currently understood as follows.

```text
ELLE
  ↓
creates / updates GOSSIP [GRAY]
  ↓
SHARON
  ↓
ERIE notices unresolved Gossip
  ↓
ERIE checks existing CHRONOS summaries
```

A CHRONOS-summary hit is a relevance signal, not epistemic resolution.

If ERIE already has something potentially relevant, the next conceptual question is:

> **How urgently is this understanding needed?**

ELLE's maturity pressure provides the developmental demand signal.

```text
LOW PRESSURE
  → retain the hit / remain unresolved / no expensive retrieval

HIGH ENOUGH PRESSURE
  → justify deeper ERIE retrieval or investigation
```

ERIE then performs epistemic work and returns grounded material with provenance.

ELLE combines that grounded result with accumulated experience and owns the developmental judgment.

The compact relationship is:

> **ELLE gives ERIE attention.**
>
> **ERIE gives ELLE knowledge.**

Experience determines what is worth understanding.

Evidence constrains what experience is allowed to teach.

---

# 14. Temporal Requirements

ELLE needs developmental notions of time, but it is not yet established whether this should be implemented as a narrow dependency on TEMPUS/CHRONOS or as smaller ELLE-local mechanics.

Relevant deterministic measures include:

- event order;
- first seen;
- last seen;
- elapsed time;
- time between occurrences;
- relevant events between occurrences;
- applicable opportunities between occurrences;
- recurrence;
- unresolved duration;
- support/contradiction spacing;
- before/after learning relationships.

An important distinction is:

> Clock time passing without a relevant opportunity should not necessarily weaken unresolved learning.

Temporal gap and experiential gap are not identical.

---

# 15. Provenance and Auditable Emergence

ELLE should preserve developmental ancestry rather than rewriting history after the fact.

Conceptually:

```text
BEHAVIOR
  ← RULE
  ← CONCLUSION
  ← GOSSIP / ASSESSMENTS
  ← PARCEL
  ← EVENT
```

When ERIE contributes evidence, the evidence and its provenance join that ancestry.

The intended property is **auditable emergence**:

A persona may change through experience, but the path by which it changed remains inspectable.

This includes rejected hypotheses, contradictions, revisions, and unresolved state.

---

# 16. Established Architectural Principles

The following are current conceptual principles of ELLE:

- ELLE externalizes learning from any single language model.
- ERIE externalizes knowing; ELLE externalizes learning.
- Models provide semantic cognition; ELLE provides continuity and deterministic developmental machinery.
- Measure deterministically; judge intelligently.
- Pressure schedules cognition; cognition makes the judgment.
- Concerns authorize attention rather than predetermine conclusions.
- Gossip is the unresolved object; GRAY is its unresolved state.
- SHARON is the shared ERIE/ELLE surface, not an actor.
- ERIE owns epistemic grounding; ELLE owns developmental maturation.
- Explicit authoritative instructions can bypass artificial maturity delay and become Rules directly when scope and meaning are clear.
- Failed suspicions and rejected hypotheses remain developmental data.
- Mature learning should compile down into small active Rules rather than forcing the full developmental history into every model context.
- Project-specific learning must be capable of remaining project-scoped.
- A Bill may be proposed for LAW consideration, but ELLE cannot enact LAW automatically.

---

# 17. Intentionally Unresolved

The following should remain unresolved until explicitly designed:

- exact Parcel schema;
- exact Gossip schema;
- exact SHARON implementation;
- exact ERIE/ELLE exchange contract;
- exact maturity-pressure formula;
- exact thresholds;
- exact browser interception/injection mechanism;
- provider-specific browser adapters;
- exact persistence technology;
- exact Concern taxonomy;
- exact Rule storage format beyond the compact durable-learning concept;
- scopes beyond broader/persona and project;
- exact Bill review lifecycle;
- whether ELLE uses a narrow TEMPUS/CHRONOS dependency or local developmental-time mechanics;
- repository module/folder structure for implementation.

These are architectural GRAYs, not permission to silently choose conventional answers.
