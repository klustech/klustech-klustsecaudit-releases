# KlustSecAudit — Windows installation (v0.3.0 Research Preview)

**Available now:** [Download `v0.3.0-preview.1`](https://github.com/klustech/klustech-klustsecaudit-releases/releases/tag/v0.3.0-preview.1). This is an **unsigned research preview**, not a production-certified installer. Refresh reinstallation on an existing Windows PC was successful with audit history intact. **A completely clean-machine installation is still unverified.**

## Requirements

- Windows 10 x64 build 19045 or later, or Windows 11 x64.
- Hardware virtualization and WSL2 support, with permission to enable Windows features.
- At least **8 GB RAM** (16 GB recommended) and about **20 GB of free space**.
- Internet for initial prerequisite downloads. Local AI can operate offline after installation.
- Administrator approval when required by Windows.

## Download and verify

1. Download [`KlustSecAudit_0.3.0_x64-setup.exe`](https://github.com/klustech/klustech-klustsecaudit-releases/releases/download/v0.3.0-preview.1/KlustSecAudit_0.3.0_x64-setup.exe).
2. Download [`SHA256SUMS.txt`](https://github.com/klustech/klustech-klustsecaudit-releases/releases/download/v0.3.0-preview.1/SHA256SUMS.txt) from the **same release**.
3. In Windows PowerShell, go to the download folder and calculate the checksum:

   ```powershell
   Get-FileHash "$HOME\Downloads\KlustSecAudit_0.3.0_x64-setup.exe" -Algorithm SHA256
   ```

4. Compare the resulting full SHA-256 with the checksum file. **For this release**, the expected SHA-256 is:

   ```
   6ECC18951359FB38F7CEBF93FCBAB24C9259C74E8132A4AC69BF1738C2EC43B3
   ```

   Do not run the installer if the values differ.

## Set up the app

1. Run the installer. It is currently unsigned: Windows may issue a warning; proceed only if you trust the publisher and have verified the downloaded file. Do not circumvent employer or organization policies.
2. Open **KlustSecAudit Desktop Setup** and choose **Check Windows**.
3. Approve setup stages as needed for WSL2, managed Ubuntu, Linux runtime, Docker, Ollama and tooling. A Windows restart may be necessary.
4. Select **Verify environment → Start backend → Open dashboard**.
5. Import only source code you own or are authorized to review.

Do not expose the local backend to the internet. Optional cloud AI providers require their own keys, explicit consent to send scoped code excerpts, and may charge separately.

## Protect existing work

When refreshing or upgrading an existing installation, **verify a Backup & Recovery backup first**. Never delete, unregister, recreate or reset an existing WSL environment to troubleshoot without first preserving your data. Source snapshots, audit records and proof evidence may reside in WSL.

## Known limitations

- Fresh installation on a separate Windows computer or clean VM has not passed acceptance testing.
- Rootless sandbox functionality depends on properly installed and approved toolchains and local environment.
- A compiling contract, successful deployment smoke test or clean static scan **does not** establish security.
- AI findings and exploit hypotheses remain unverified without adequate independent proof and human review.

For bugs, use [GitHub Issues](https://github.com/klustech/klustech-klustsecaudit-releases/issues/new/choose) and share only **redacted**, non-sensitive diagnostics.
