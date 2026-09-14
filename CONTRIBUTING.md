# Contributing

This repository is the archival package for a Zenodo-deposited technical
note:

> Rolando Bosch, "Behavioral Canarying for Prompt Injection: Powerless Model
> Probes with Explicit Coverage Semantics," Zenodo technical note (2026).
> <https://doi.org/10.5281/zenodo.21818564>

It exists to preserve the paper, its citation records, and its metadata in a
stable, versioned location. It is not a software project, and it does not
take feature contributions, pull requests implementing new functionality, or
issues about desired behavior.

## What belongs here

- Corrections to the archived paper text (typos, factual errors, broken
  links) that do not change its substantive claims.
- Corrections to `CITATION.cff`, `CITATION.bib`, `codemeta.json`,
  `.zenodo.json`, `metadata.json`, or other citation and metadata records.
- Corrections to this README or the files listed in it (for example a stale
  DOI, checksum, or cross-link).

Open an issue or a small pull request for any of the above.

## What does not belong here

This architecture is operationalized by a separate, independent repository:
[Little Canary](https://github.com/hermes-labs-ai/little-canary), the
open-source reference implementation described in this paper. Bug reports,
feature requests, and any implementation-level discussion belong in that
repository, not here.

There is no development workflow, test suite, or review SLA for this
repository — it is a static archive, and changes are limited to the
corrections described above.
