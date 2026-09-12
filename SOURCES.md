# Sources for behavioral-canarying template

Every value in this folder traces to one of the URLs below. Nothing is
invented; where a value could not be verified (e.g. current GitHub topics),
the file says so explicitly instead of guessing.

| Field | Value | Source |
|---|---|---|
| Title | "Behavioral Canarying for Prompt Injection: Powerless Model Probes with Explicit Coverage Semantics" | https://zenodo.org/api/records/21820059 (`metadata.title`) |
| Concept DOI | 10.5281/zenodo.21818564 | https://zenodo.org/api/records/21820059 (`conceptdoi`) |
| Version DOI | 10.5281/zenodo.21820059 | https://zenodo.org/api/records/21820059 (`doi`) |
| Version | 1.0.1 | https://zenodo.org/api/records/21820059 (`metadata.version`) |
| Publication date | 2026-08-06 | https://zenodo.org/api/records/21820059 (`metadata.publication_date`) |
| Resource type | Technical note (publication/technicalnote) | https://zenodo.org/api/records/21820059 (`metadata.resource_type`) |
| Author | Bosch, Rolando; Hermes Labs; ORCID 0009-0005-4896-1112 | https://zenodo.org/api/records/21820059 (`metadata.creators`) |
| License | CC BY 4.0 (`cc-by-4.0`) | https://zenodo.org/api/records/21820059 (`metadata.license`) |
| Keywords | prompt injection; behavioral canarying; AI agent security; fail-open systems | https://zenodo.org/api/records/21820059 (`metadata.keywords`) |
| Abstract text | as quoted in README.md and CITATION.cff | https://zenodo.org/api/records/21820059 (`metadata.description`, HTML tags stripped) |
| Related identifier | https://github.com/hermes-labs-ai/little-canary (isSupplementedBy, software) | https://zenodo.org/api/records/21820059 (`metadata.related_identifiers`) |
| PDF filename / size | behavioral-canarying-technical-note-v1.0.1.pdf, 621,609 bytes | https://zenodo.org/api/records/21820059 (`files[0]`) |
| Canonical HTML edition | https://hermes-labs.ai/research/behavioral-canarying | live fetch of that URL, 2026-09-11; also `path` field in /home/user/hermes-labs-v2/src/lib/research-papers.ts (`BEHAVIORAL_CANARYING.path`) |
| Hosted PDF URL | https://hermes-labs.ai/papers/behavioral-canarying-technical-note-v1.0.1.pdf | /home/user/hermes-labs-v2/src/lib/research-papers.ts (`BEHAVIORAL_CANARYING.pdfPath`), confirmed listed in https://hermes-labs.ai/sitemap.xml |
| "Operationalizing tool repository" framing (no dedicated paper-archive repo exists) | https://github.com/hermes-labs-ai/little-canary | /home/user/hermes-labs-v2/src/lib/research-papers.ts (`BEHAVIORAL_CANARYING.githubUrl`); confirmed by hermes-publications README.md and publications.json (`archive_repository` field), commit 738fd6edadab1542447ffc98141c3c19dadde4df of https://github.com/hermes-labs-ai/hermes-publications, cloned read-only into scratchpad |
| Repository-naming convention (bare slug, matching site path) | e.g. hermes-labs-ai/the-asymmetric-burden-of-proof, hermes-labs-ai/precise-records-unstable-meanings, hermes-labs-ai/the-generative-horizon | local checkouts at /home/user/the-asymmetric-burden-of-proof, /home/user/precise-records-unstable-meanings, and the-generative-horizon cloned read-only (`git remote -v` on each) |
| Standard file set (README/CITATION.cff/CITATION.bib/LICENSE.md/metadata.json/SHA256SUMS pattern) | modeled on the four existing paper repos | direct file listing of /home/user/the-asymmetric-burden-of-proof, /home/user/taxonomy-of-epistemic-failure-modes, /home/user/precise-records-unstable-meanings, and the cloned the-generative-horizon |
| Common-core topics (ai-agents, ai-reliability, epistemic-engineering, hermes-labs, research-paper) | present on all four existing paper repos | `curl https://api.github.com/repos/hermes-labs-ai/<repo>` (public, unauthenticated, works for public repos despite the GitHub *search* API being unavailable to this session) fetched live 2026-09-11 for `the-asymmetric-burden-of-proof`, `taxonomy-of-epistemic-failure-modes`, `precise-records-unstable-meanings`, `the-generative-horizon` — each returned a `topics` array containing all five |
| prompt-injection, agent-security, ai-safety, llm-security | topics already used on the operationalizing tool repo | same live call against `https://api.github.com/repos/hermes-labs-ai/little-canary`, `topics` field |

## Caution recorded, not a sourced fact

The `.zenodo.json` file's `_comment` field is this session's own recommendation
(not a citation) that GitHub→Zenodo webhook integration stay OFF for this
repository, because the paper already has a canonical Zenodo deposit created
directly; enabling the integration on a later GitHub release would mint a
second, duplicate DOI rather than referencing 10.5281/zenodo.21818564. Verify
this against Zenodo's own GitHub integration documentation before enabling any
integration.
