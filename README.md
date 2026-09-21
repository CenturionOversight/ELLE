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

## Public architecture boundary

ELLE sits outside any individual model and preserves developmental continuity across model interactions.

Its public contract is intentionally narrow:

- experience can accumulate into durable learning;
- unresolved learning remains unresolved until it earns judgment;
- learned behavior is scoped and attributable;
- developmental history remains inspectable; and
- model providers remain replaceable.

The mechanisms that implement that contract — internal topology, schemas, exchange contracts, persistence design, pressure mechanics, integration protocols, and orchestration — are proprietary VOLSHi architecture and are not documented here.

## Relationship with ERIE

ERIE and ELLE are developmental twins with deliberately separate authority.

> **ERIE externalizes knowing. ELLE externalizes learning.**

ERIE grounds what the available evidence supports. ELLE preserves what experience has earned the right to change. Neither substitutes for the other, and neither requires a particular model provider.

## Status

ELLE is an **active VOLSHi engine under development**, not a conceptual research placeholder.

The architecture is established and implementation work is underway on the external learning engine: developmental state, scope isolation, provenance and ancestry, maturation, Rule formation, and the deterministic boundaries that support model-assisted judgment.

ELLE is being built as a Python 3.11+ engine with its core implementation under `src/elle/`. The browser-edge bridge is one integration surface around that engine; it is not ELLE itself.

The current development boundary preserves the distinction with ERIE: ERIE externalizes knowing; ELLE externalizes learning. Implementation is focused on making that developmental continuity durable, inspectable, and independent of any replaceable model backend.

Detailed internal architecture is maintained privately. This repository documents ELLE's purpose, public boundary, and externally relevant behavior.

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
