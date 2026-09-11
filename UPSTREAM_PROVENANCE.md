# OpenWork Import and Provenance Policy

> Status: Normative import policy; no source imported during documentation phase
> Governing decision: ADR-0018

## Selected boundary

The evaluated upstream is `https://github.com/different-ai/openwork`. Only
MIT-licensed desktop and core files outside `ee/` are eligible. Den, hosted MCP,
hosted inference, enterprise-only code, hosted accounts and upstream telemetry are
excluded. The research snapshot was `dev` at
`0b219dc4e5f2868c258dbe960d58c657dbe8d99b`, observed 2026-09-10; observation
does not itself authorize copying.

## Implementation import gate

The pull request that imports source SHALL pin the exact immutable commit and
archive checksum; inventory imported, removed, generated and vendored files;
preserve notices; prove excluded paths and capabilities are absent; lock
dependencies; produce license, SBOM and vulnerability reports; review Electron,
IPC, updater, local server, workspace and tool threats; pass supported-OS and
accessibility tests; implement Commons gateway and session adapters; and name the
responsible release and vulnerability owners.

If any requirement fails, the desktop client SHALL use a clean implementation of
the PSDC Desktop contracts. The architecture is complete independently of whether
the evaluated upstream is ultimately imported.
