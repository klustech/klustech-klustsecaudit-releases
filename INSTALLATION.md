# KlustSecAudit — Windows installation (research preview)

> **No public installer is available yet.** This page describes prerequisites and the planned setup experience; clean-machine installation has not yet passed release acceptance.

## Requirements

- Windows 10 x64 build 19045 or newer, or Windows 11 x64.
- Hardware virtualization enabled, with permission to set up WSL2.
- At least **8 GB RAM** (16 GB recommended) and approximately **20 GB free disk space**.
- Internet access during prerequisite setup; local/offline auditing is possible after the required components and model are installed.
- Administrator approval when Windows needs to enable WSL2 or other OS features.

## Planned setup

1. Download the installer from [GitHub Releases](https://github.com/klustech/klustech-klustsecaudit-releases/releases) **once a release exists**.
2. Check the installer SHA-256 against the checksum included with the release.
3. Launch the Windows installer. Early research builds may be unsigned: review any Windows warning and proceed only if you trust the source.
4. Open **KlustSecAudit Desktop Setup**, then use **Check Windows**.
5. Approve each required setup stage separately: WSL2, managed Ubuntu, Linux runtime, Docker/Ollama and model tools where applicable. Windows might request a restart.
6. Choose **Verify environment**, then **Start backend → Open dashboard**.
7. Import only smart contracts you are authorized to test.

The UI does not grant permission to test third-party systems. Backend, AI, and rootless sandbox readiness must be checked separately. Optional OpenAI/Anthropic inference requires an API key and explicit permission to transmit selected source excerpts; it may incur charges.

## Data preservation

Before reinstalling or upgrading, use the application's **Backup & Recovery** controls and verify the backup. Do not delete an existing WSL distribution, database, evidence store, model, or audit history to troubleshoot the preview.

## Limitations

- The installer is not yet validated on a second clean Windows computer.
- Foundry/Slither sandbox execution requires approved, correctly installed tools.
- No automatic vulnerability verification or guaranteed exploit discovery is provided.
- Never publish API keys, contract secrets, customer source code, or private audit evidence in GitHub issues.

For reporting installation problems after a public release, open an [issue](https://github.com/klustech/klustech-klustsecaudit-releases/issues) with the installer version, Windows version, and redacted logs.
