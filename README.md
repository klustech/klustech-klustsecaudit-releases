# KlustSecAudit — Desktop Smart Contract Security Workbench

**Status: Research preview — public installer not released yet.**

KlustSecAudit is a Windows desktop application for **authorized** Ethereum/EVM smart contract security research. It brings Solidity source inspection, static analysis, AI-assisted investigation, bounded local testing, and evidence-backed reporting into a single desktop workflow.

> **Important:** KlustSecAudit is a research tool, **not** a certified auditor or an autonomous exploit-discovery system. Findings are provisional until independently reviewed and reproduced. A clean scan does not establish security.

## Capabilities

- Import authorized Solidity sources from ZIP files, local projects, or supported public repositories.
- Browse source snapshots and source-linked research notes.
- Compile Solidity and run Slither static analysis when the approved toolchain is installed.
- Run bounded Foundry tests and review reproducible evidence in supported proof workflows.
- Investigate with **local Ollama** or **optional** external OpenAI/Anthropic APIs with explicit consent and independent API billing.
- Export audit reports, results, and integrity evidence.

## Download and availability

The first public installer is **not yet published**. When validation is complete, it will appear on the [Releases page](https://github.com/klustech/klustech-klustsecaudit-releases/releases).

The initial distribution is planned for **Windows x64**. The installer may be **unsigned**, and Windows may display a publisher warning. Do not bypass organizational security policies. Before installing any release, check its published SHA-256 checksum.

For system requirements and the planned graphical setup process, see [Installation](INSTALLATION.md).

## Known limitations

- Independent exploit-discovery accuracy has **not** been demonstrated by a sufficient controlled benchmark.
- Detected candidates, AI assessments, and proof artifacts **are not automatically verified vulnerabilities**.
- Local tool execution and AI model availability depend on correctly installed and authorized prerequisites.
- A successfully built installer does not guarantee a successful clean-machine installation or complete recovery.
- Do not use this research preview as the sole basis for protecting or deploying financial contracts.

## Privacy and responsible use

The desktop workflow is designed for local, loopback-bound operation. Local Ollama inference can remain offline. If an external AI provider is selected, scoped source excerpts are sent to that provider **only with explicit approval**, and API charges may apply.

Audit only software you own or are authorized to assess. Do not put private keys, credentials, or confidential customer code into public GitHub issues.

## Feedback

After the first release, please use [Issues](https://github.com/klustech/klustech-klustsecaudit-releases/issues) for installation problems, reproducible bugs, and feature feedback. Include the release version and non-sensitive diagnostic information.

## Source code and licensing

This repository is for **public binary distributions and release documentation**. It does **not** contain the KlustSecAudit application source, which remains private. The public availability of this repository does not by itself license the proprietary application source or authorize redistribution of binaries. Applicable binary-use terms will be supplied before the first download.

**Developed by Klustertech.**
