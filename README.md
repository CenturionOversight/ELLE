# ELLE

**External Learning Loop Engine — persistent developmental learning outside the model.**

ELLE is VOLSHi's developmental-learning infrastructure: a model-independent engine for preserving how intelligent systems learn from experience over time.

Instead of leaving learning trapped in model weights, prompts, or disposable context windows, ELLE makes developmental continuity persistent system state. Experience, unresolved learning, maturation, provenance, scope, and durable behavioral Rules can survive the model that helped interpret them.

ELLE is the developmental learning engine in the ARCHETRON ecosystem and the learning side of VOLSHi's span between machine intelligence and human experience.

Its fundamental question is:

> **What did I learn, and why?**

ELLE externalizes learning from any individual language model. A model may reason, interpret, and judge, but ELLE preserves the developmental continuity: what happened, what was considered, what remains unresolved, what matured into a conclusion, and what has earned the right to influence future behavior.

That makes the model replaceable without making the persona development disposable.

## Core distinction

ERIE and ELLE are twin engines with different authority.

**[ERIE — Epistemic Retrieval & Intelligence Engine](https://github.com/ArchePersona/ERIE-info)** asks:

> **What do I know, and why?**

**ELLE — External Learning Loop Engine** asks:

> **What did I learn, and why?**

ERIE owns evidence, retrieval, provenance, and epistemic grounding.

ELLE owns developmental interpretation, maturation, and learned behavioral continuity.

> **ERIE externalizes knowing. ELLE externalizes learning.**

> **Evidence earns conclusions. Experience earns rules.**

## Operating principle

ELLE uses deterministic machinery wherever computation is sufficient and reserves model cognition for actual interpretation and judgment.

> **Measure deterministically. Judge intelligently.**

Pressure does not make the learning decision. Pressure decides when a question has earned another look.

> **Pressure schedules cognition. Cognition makes the judgment.**

## Runtime position

ELLE is a learning-control layer around model interaction.

The browser can act as the edge bridge: observing the conversation, attaching small ELLE instructions to an outbound model call, receiving ELLE-only structured return data, stripping that metadata from the visible conversation, and caching the active learning state needed for the next turn.

ELLE itself is not merely a browser extension. Durable developmental state belongs outside the transient page.

```text
USER
  ↓
BROWSER / CHAT UI
  ↓
ELLE BRIDGE
  ↓
ACTIVE ELLE CONTEXT
  ↓
LLM
  ↓
ELLE-ONLY STRUCTURED RETURN
  ↓
ELLE STATE / SHARON / ERIE
  ↓
NEXT TURN
```

## Core primitives

- **Parcel** — ELLE's traveling developmental work object.
- **Concern** — authorization to pay attention to a dimension of possible improvement.
- **Procedure** — the concern-specific method used to assess what happened.
- **Gossip** — a first-class unresolved learning object.
- **GRAY** — the unresolved state of Gossip.
- **SHARON** — the shared surface where ELLE and ERIE exchange Gossip; the "treehouse."
- **Rule** — a compact durable lesson that has earned the right to influence future behavior.
- **Project Rule** — a Rule whose authority is limited to a project scope.
- **Bill** — a proposal for possible LAW consideration. A Bill is not a LAW.

## Conceptual learning flow

```text
EVENT
  ↓
PARCEL
  ↓
APPLICABLE CONCERN
  ↓
PROCEDURE
  ↓
ASSESSMENT
  ├─ established → conclusion → rule
  └─ unresolved  → gossip [GRAY] → SHARON
```

The slower developmental path is:

```text
EXPERIENCE
  ↓
GOSSIP [GRAY]
  ↓
SUPPORT / CONTRADICTION / QUALIFICATION
  ↓
DETERMINISTIC MATURITY PRESSURE
  ↓
MODEL JUDGMENT WHEN WARRANTED
  ↓
REMAIN GRAY / REJECT / CONCLUDE
  ↓
RULE
```

Explicit authoritative instruction can take a fast path when authority, scope, and meaning are already clear:

```text
AUTHORITATIVE INSTRUCTION
  ↓
RULE
```

ELLE should not manufacture uncertainty merely to simulate learning.

## The twin relationship

SHARON is the shared surface. GOSSIP is the shared unresolved object. GRAY is its unresolved state.

When ELLE creates new Gossip, ERIE can first check knowledge it already has summarized through CHRONOS. A relevant summary hit is an opportunity signal, not proof and not an automatic request for expensive retrieval.

ERIE can effectively ask:

> **How urgently is this understanding needed?**

ELLE's accumulated developmental pressure provides the demand signal.

Low pressure can leave the Gossip unresolved without spending more resources. Higher pressure can justify a deeper ERIE investigation. ERIE returns grounded evidence and provenance. ELLE combines that grounding with accumulated experience and owns the learning judgment.

> **ELLE gives ERIE attention. ERIE gives ELLE knowledge.**

ERIE does not decide what ELLE learns. ELLE does not decide what ERIE's evidence proves.

## Developmental history

ELLE does not erase failed learning attempts simply because they did not mature.

A suspicion that was rejected is still developmental data. Contradictions, revisions, rejected hypotheses, and failed interpretations remain part of the provenance chain.

The intended ancestry is inspectable:

```text
behavior
  ← rule
  ← conclusion
  ← gossip / assessments
  ← parcel
  ← event
```

Where ERIE participates, grounded evidence and provenance join that ancestry.

The desired result is **auditable emergence**: a persona can change through accumulated experience while the path by which it changed remains inspectable.

## Status

ELLE is an **active VOLSHi engine under development**, not a conceptual research placeholder.

The architecture is established and implementation work is underway on the external learning engine: developmental state, scope isolation, provenance and ancestry, maturation, Rule formation, and the deterministic boundaries that support model-assisted judgment.

ELLE is being built as a Python 3.11+ engine with its core implementation under `src/elle/`. The browser-edge bridge is one integration surface around that engine; it is not ELLE itself.

The current development boundary preserves the distinction with ERIE: ERIE externalizes knowing; ELLE externalizes learning. Implementation is focused on making that developmental continuity durable, inspectable, and independent of any replaceable model backend.

See [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) for the architecture record.

## Explore ARCHETRON

- [ARCHETRON](https://github.com/CenturionOversight/ARCHETRON) — the VOLSHi technology ecosystem
- [ERIE](https://github.com/ArchePersona/ERIE-info) — evidence, knowledge, and investigation
- [ARCHE](https://github.com/ArchePersona/ARCHE-info) — attention allocation
- [PEEP](https://github.com/ArchePersona/PEEP-info) — execution observation
- [RATTER](https://github.com/ArchePersona/RATTER-info) — operational telemetry
- [SHERLOCK](https://github.com/ArchePersona/SHERLOCK-info) — evidence-driven reconstruction and investigation
- [ARCHEMADA](https://github.com/ArchePersona/ARCHEMADA-info) — controlled AI-assisted software construction
- [ARCHESTRATOR](https://github.com/CenturionOversight/ARCHESTRATOR-info) — software engineering lifecycle infrastructure
- [DEVSnitcher](https://github.com/CenturionOversight/devsnitcher) — browser-edge evidence capture
