<!--
GENERATED FILE — do not edit directly.
Generated from the repository's pinned public instruction contract.
profile:  emm-public-documentation
revision: agents-contract-v2.0.0
fragments:
  - documentation-contract (sha256:401a2c3f9ed2)
  - public-repository-boundary (sha256:13b121d6df71)
  - release-publication-contract (sha256:a0cd1b33cb49)
-->

## Documentation Requirements
- Lead every substantial page with a short TL;DR that states the outcome, audience, prerequisites, and the next action.
- Structure documentation from a holistic index into progressively detailed architecture, setup, operator, API, security, and troubleshooting pages. Avoid multiple competing entry points for the same procedure.
- Use short step-by-step guides where an operator must create files, secrets, certificates, databases, deployment packages, backups, or rollback artifacts.
- Distinguish product overview, application architecture, backend architecture, networking/data exchange, setup, developer workflow, deployment/operator procedure, API/contracts, security, and evidence. Link between owners instead of duplicating a drifting copy.
- Architecture documentation covers components, ownership, interfaces, data models, class/component views, runtime/sequence views, external dependencies, security boundaries, and failure behavior.
- Operator documentation follows the real lifecycle: choose a lane, plan and pin, verify, package, configure secrets/trust, deploy, validate, promote, observe, update/rollback, back up, and recover.
- State clearly which lanes are implemented, experimental, future, or unsupported. Documentation must never claim a runnable deployment, security property, or recovery path that has not been verified.
- Keep pages current in the same slice as the code or contract they explain. Remove obsolete procedures and repair indexes when ownership or paths change.
- Documentation-only work does not run unrelated builds or tests. Validate links, diagrams, examples, and generated-document contracts appropriate to the edited pages.

## Public Repository Boundary
- Keep instructions and documentation self-contained for a public reader. Do not reference private sibling paths, private repositories, internal model maps, private delivery procedures, or unavailable organizational tooling.
- Never publish secrets, credentials, private endpoints, customer or operator data, internal incident details, private evidence notes, or security-sensitive infrastructure topology.
- Public examples use non-sensitive placeholder values and explain which values an adopter must supply.
- Public release, contribution, setup, and security instructions describe only workflows that external users can actually access.
- If a change depends on private context, keep that context in the private owner and publish only the minimum stable public contract needed by this repository.

## Release Publication Requirements
- A GitHub release entry is part of the released artifact. Creating or moving only a Git tag does not complete a release.
- In a repository with one release stream, the GitHub release title equals the exact Git tag, including its case, separators, and version prefix.
- A repository with multiple independently versioned release streams may title an entry `<stream>-<tag>`, where `stream` uses lowercase words separated only by hyphens. Do not add a second prefix when the tag already identifies its stream.
- Do not use display names, title case, spaces, or descriptive prose in a release title. Put human-readable context in the release notes.
- Release notes state the material changes, compatibility or migration impact, verification evidence, and known limitations appropriate to the repository.
- Work that changes a versioned artifact uses a feature or integration branch and a pull request. After the branch reaches a coherent state and merges, publish the next warranted version; do not leave release-worthy changes indefinitely on the designated base without a release.
- Before declaring multi-repository delivery complete, verify every changed versioned artifact has its required immutable tag and correctly titled release entry.
