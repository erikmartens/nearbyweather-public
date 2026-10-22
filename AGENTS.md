<!--
GENERATED reviewed projection; do not edit. Human source remains authoritative.
profile: emm-public-documentation; revision: agents-contract-v4.2.1
Source/projection checksums: .agents/contract.lock
-->

## Instruction Ownership

- Shared behavior rules belong in canonical shared profiles, not project instructions; extend/consolidate before adding.
- Default no local rules. Only unique project/subtree constraints qualify: record uniqueness; names/paths/examples do not establish it. Never duplicate/override shared rules, including enrollment/revisits.
- Uncertain ownership: present scope/evidence for user decision; never invent local exceptions.

## Documentation Requirements

- Substantial pages start with TL;DR: outcome/audience/prerequisites/next action.
- One holistic index leads to architecture/setup/operator/API/security/troubleshooting detail; no competing procedure entries.
- Use short steps for creating files/secrets/certificates/databases/packages/backups/rollback artifacts.
- Distinguish product/app/backend/network/setup/workflow/operations/API/security/evidence docs; link owners, never duplicate drifting copies.
- Architecture covers components/owners/interfaces/data/static and runtime views/dependencies/security/failure.
- Operations follow lane choice, planning/pins, verification/package, secrets/trust, deploy/validate/promote/observe/update/rollback/backup/recovery.
- Label implemented/experimental/future/unsupported; never claim unverified deployment/security/recovery.
- Keep docs with code/contract slices; repair missing/stale owner guidance, local/companion PRs, obsolete procedures/indexes/links. Preserve proposal/merge/release/privacy boundaries.
- Docs-only: no unrelated builds/tests; validate relevant links/diagrams/examples/generated contracts.

## Public Repository Boundary

- Public instructions/docs self-contained; no private paths/repos/procedures/unavailable tooling.
- Never publish secrets/credentials/private endpoints/customer-operator data/incidents/private evidence/sensitive topology.
- Examples use safe placeholders; explain adopter-supplied values.
- Public release/contribution/setup/security workflows must be externally accessible.
- Keep private-dependent context private; publish only required stable public contract.

## Task Completion Cleanup

- Track exact task-owned paths/devices; reuse while needed, clean when finished before handoff.
- Remove task caches/intermediates/scratch only when no process/verification/review/follow-up needs them. Preserve deliverables/unique work/user files/diagnostics/in-use shared caches.
- Shut down task-launched devices/unused windows after checking other sessions need none; never stop unrelated devices or delete stored data merely for shutdown.
- Use owning cleanup tools/exact IDs, never global purges. Unclear ownership/retention: preserve and explain.
- Verify cleanup; report meaningful retained resources/failures.

## Release Publication Requirements

- Release requires GitHub entry, not tag alone.
- Single-stream release title equals exact tag, case/prefix/separators included.
- Multiple streams may use `<lowercase-hyphenated-stream>-<tag>`; do not duplicate a stream already in tag.
- No prose/display names/title case/spaces in titles; context belongs in notes.
- Notes cover material changes/compatibility/migration/verification/limits as relevant.
- Versioned changes use feature/integration PR; after coherent merge publish warranted next version. Never leave release-worthy changes indefinitely unreleased.
- Before multi-repo completion, verify every changed artifact's immutable tag and correctly titled release.
