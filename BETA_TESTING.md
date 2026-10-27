# Join the KlustSecAudit Windows Research Preview

**Version:** [v0.3.0-preview.1](https://github.com/klustech/klustech-klustsecaudit-releases/releases/tag/v0.3.0-preview.1)  
**Platform:** Windows 10 (build 19045+) or Windows 11 x64 with WSL2 / virtualization support.

We are looking for Solidity developers, smart-contract auditors, security researchers and Windows users willing to try this **free, closed-source research preview** and report what works or fails.

KlustSecAudit is a *security research workbench*—not a certified auditing system or a proven autonomous exploit detector. Treat every finding as provisional. Initial release builds are **unsigned** and clean-machine installation is still unverified.

## Try it

1. Read the [installation guide](INSTALLATION.md), download the [Windows installer](https://github.com/klustech/klustech-klustsecaudit-releases/releases/download/v0.3.0-preview.1/KlustSecAudit_0.3.0_x64-setup.exe), and verify it against [SHA256SUMS.txt](https://github.com/klustech/klustech-klustsecaudit-releases/releases/download/v0.3.0-preview.1/SHA256SUMS.txt).
2. Run the guided setup, select **Verify environment → Start backend → Open dashboard**.
3. Import a **non-confidential** sample contract you own or have permission to test.
4. If available, try source browsing, AI Researcher with **local Ollama**, a static scan, and a report export. Slither and Foundry require approved local tooling. **Cloud AI is optional and may cost money; you do not need it for beta feedback.**
5. Tell us whether setup succeeded, what you tried, where you got stuck, and whether the interface would be useful to your workflow.

## Report your experience

- **[Installation problem or bug](https://github.com/klustech/klustech-klustsecaudit-releases/issues/new?template=bug_report.md)** — include your Windows version, release version, the step that failed, what you expected, and a sanitized error message.
- **[Research feedback or feature suggestion](https://github.com/klustech/klustech-klustsecaudit-releases/issues/new?template=feedback.md)** — tell us what worked, what was confusing, and the *one change* you would value most.

A report saying **“installation failed at step X”** is helpful. So is **“installed, imported a public sample, and exported a report successfully.”** We value critical feedback and don't expect you to find an exploit.

**Privacy:** Do not publicly upload API keys, seed phrases, financial credentials, private contract code, local filesystem paths, user information, or sensitive audit evidence. Redact screenshots and diagnostics before attaching them to GitHub issues.

The public repository contains downloads and documentation only. Application source remains private; please don't describe the binary distribution as open-source software.

**Thank you for helping Klustertech test the research preview.**
