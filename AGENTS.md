<!--
GENERATED FILE — do not edit directly.
Generated from the repository's pinned public instruction contract.
profile:  emm-public-documentation
revision: agents-contract-v3.2.1
fragments:
  - instruction-ownership (sha256:8f39f4e402ab)
  - documentation-contract (sha256:401a2c3f9ed2)
  - public-repository-boundary (sha256:43d83d7d0459)
  - task-cleanup (sha256:8c824853baba)
  - release-publication-contract (sha256:a0cd1b33cb49)
-->

## Instruction Ownership
- Before adding or changing a rule, check whether it governs behavior shared across projects. Shared rules belong in the canonical shared contract repository and applicable profiles, not in a project's local instructions. Extend or consolidate an existing rule before adding another one.
- Default to zero project-local rules: most repositories should need only a shared profile and version pin, with no local rules file. Project-local rules are allowed only for a constraint unique to that project or subtree. Record what makes it unique; a project-specific example, name or path does not make a general rule local. Do not duplicate or override shared rules in local instruction files. Apply this check during enrollment and when revisiting existing local rules too.
- If shared versus project-local ownership is uncertain, present the scope and evidence to the user and let the user decide before adding the rule. Do not default uncertainty into a local exception.

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
- Keep instructions and documentation self-contained for a public reader. Do not reference private sibling paths, private repositories, private delivery procedures, or unavailable organizational tooling.
- Never publish secrets, credentials, private endpoints, customer or operator data, internal incident details, private evidence notes, or security-sensitive infrastructure topology.
- Public examples use non-sensitive placeholder values and explain which values an adopter must supply.
- Public release, contribution, setup, and security instructions describe only workflows that external users can actually access.
- If a change depends on private context, keep that context in the private owner and publish only the minimum stable public contract needed by this repository.

## Task Completion Cleanup
- Track temporary paths and simulator or emulator identifiers created or launched for the task. Reuse them while needed, then clean up resources whose work has finished before the final handoff.
- Prune task-owned caches, build intermediates, scratch files and disposable output once no running process, verification, review or follow-up needs them. Preserve deliverables, unique work, user files, required diagnostic evidence and shared caches still in use; completion alone does not make every output disposable.
- Shut down simulators and emulators launched for completed task processes after confirming that no other task or user session still needs them. Close their unused windows without stopping unrelated devices or sessions; shutting down a simulator does not require deleting its device or stored data.
- Use exact task-owned paths and resource identifiers with the owning tool's cleanup mechanism. Do not blanket-purge global caches, temporary directories or simulator fleets. When ownership or retention is unclear, leave the resource intact and note why it remains.
- Verify that cleanup succeeded. Include any meaningful retained resources or cleanup failures in the handoff so they can be resolved without losing work.

## Release Publication Requirements
- A GitHub release entry is part of the released artifact. Creating or moving only a Git tag does not complete a release.
- In a repository with one release stream, the GitHub release title equals the exact Git tag, including its case, separators, and version prefix.
- A repository with multiple independently versioned release streams may title an entry `<stream>-<tag>`, where `stream` uses lowercase words separated only by hyphens. Do not add a second prefix when the tag already identifies its stream.
- Do not use display names, title case, spaces, or descriptive prose in a release title. Put human-readable context in the release notes.
- Release notes state the material changes, compatibility or migration impact, verification evidence, and known limitations appropriate to the repository.
- Work that changes a versioned artifact uses a feature or integration branch and a pull request. After the branch reaches a coherent state and merges, publish the next warranted version; do not leave release-worthy changes indefinitely on the designated base without a release.
- Before declaring multi-repository delivery complete, verify every changed versioned artifact has its required immutable tag and correctly titled release entry.
