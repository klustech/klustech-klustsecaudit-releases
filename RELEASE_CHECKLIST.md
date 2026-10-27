# First public release checklist

**Target:** KlustSecAudit v0.3.0 **Research Preview** — do not label stable or independently security-certified.

- [ ] Freeze the private source revision used for the release (record Git commit).
- [ ] Run Python, frontend, native packaging, and targeted installation checks from that revision.
- [ ] Verify the installer contains no API keys, private audit databases, real customer sources, local absolute paths or sensitive evidence.
- [ ] Install on an independent clean Windows x64 machine or VM with supported virtualization.
- [ ] Verify graphical WSL2/backend setup, audit import, local analysis, export, and safe restart without destroying user data.
- [ ] Run an authorized sample through compile, static scan, and available Foundry tooling; record any limitation.
- [ ] Confirm Backup & Recovery behavior; retain a known-good restore path.
- [ ] Decide and include binary-use terms; review redistribution/licensing obligations for bundled dependencies.
- [ ] Produce the final `.exe` and its SHA-256 checksum from the **same frozen build**.
- [ ] Clearly identify unsigned installation and unconfigured updates; do not imply publisher signing.
- [ ] Add release notes that explain working features, known limitations, Windows/WSL prerequisites, and security disclaimer.
- [ ] Publish **as a GitHub prerelease**, not a stable release.
- [ ] Verify that public downloads work and the release repository exposes **no private application source**.

**Policy:** Passing a build is not passing clean-machine release acceptance. The first public release should proceed only when its installation claims have been tested or explicitly qualified.
