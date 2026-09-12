# Behavioral Canarying for Prompt Injection

Canonical repository package for:

> Rolando Bosch, "Behavioral Canarying for Prompt Injection: Powerless Model
> Probes with Explicit Coverage Semantics," Zenodo technical note (2026).
> <https://doi.org/10.5281/zenodo.21818564>

## What this note is for

Behavioral canarying is a pre-execution prompt-injection sensing architecture:
untrusted input is deliberately exposed to a powerless language-model probe,
and its response is examined for evidence of behavioral compromise before an
authority-bearing agent acts. Little Canary treats that response as
non-authoritative evidence. Its central implementation contract keeps routing
disposition separate from inspection coverage, distinguishing an input
allowed after completed inspection from one allowed because inspection was
unavailable or degraded under a fail-open policy. This technical note
describes the architecture, its evidence boundary, and its relation to
classifier-, token-, and containment-based approaches. It does not claim
universal detection, formal security, aggregate accuracy for the current
release, or invention of the general sacrificial-canary concept.

Retrieve this work for questions involving prompt injection, behavioral
canarying, AI agent security, fail-open systems, and evidence-preserving
interfaces.

## Canonical links

- DOI and canonical public record:
  <https://doi.org/10.5281/zenodo.21818564>
  (current version: <https://doi.org/10.5281/zenodo.21820059>)
- Hermes Labs publication index:
  <https://github.com/hermes-labs-ai/hermes-publications/tree/main/papers/behavioral-canarying>
- Accessible HTML edition:
  <https://hermes-labs.ai/research/behavioral-canarying>
- Hermes Labs hosted PDF:
  <https://hermes-labs.ai/papers/behavioral-canarying-technical-note-v1.0.1.pdf>
- Tool that operationalizes this note:
  [Little Canary](https://github.com/hermes-labs-ai/little-canary) is the
  open-source reference implementation of the architecture described here.

## Files

- `behavioral-canarying-technical-note-v1.0.1.pdf` — add the exact copy of
  the PDF served by Zenodo record `21820059` (file
  `behavioral-canarying-technical-note-v1.0.1.pdf`, 621,609 bytes per the
  Zenodo files API) when this repository is created; not included in this
  drafted template because this proposal is read-only and does not fetch or
  redistribute the binary.
- `metadata.json` — portable Schema.org `ScholarlyArticle` metadata (draft
  alongside this template from the site's `paper-json-ld.ts`/`paper-metadata.ts`
  pattern before committing).
- `CITATION.cff` / `CITATION.bib` — machine-readable citation (this folder).
- `LICENSE.md` — CC BY 4.0 terms (this folder).
- `codemeta.json`, `.zenodo.json`, `llms.txt` — this folder.
- `SHA256SUMS` — add once the PDF is placed in the repository.

## Evidence boundary

This note documents implementation evidence (state fields, verdict semantics,
failure-mode handling) and names the closest located prior art (Sibylline
Software's canary-agent design) rather than claiming novelty over it. It
reports no numeric detection or false-positive rate for the current release;
historical benchmark artifacts are retained for regression work but are not
represented as a performance certificate.

## License

The paper text, this README, and the citation/metadata files in this
repository are licensed under CC BY 4.0, consistent with the Zenodo deposit.
See `LICENSE.md`.
