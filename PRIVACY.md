# BesaGuard beta privacy

BesaGuard performs its current scanning and observation workflows locally on the computer. Findings, preferences, development telemetry snapshots, and encrypted holding copies remain under the current user's `%LocalAppData%\BesaGuard` directory.

The application contacts the public `promptedteam/BesaGuard` GitHub repository once after startup to read the small beta update manifest. It contacts GitHub again only if the user presses **Check again** or explicitly downloads an available installer. Those requests are subject to GitHub's own privacy terms and normal network logging. BesaGuard does not upload scanned files, findings, file paths, or holding-vault contents through its update channel.

The hardened update client in newer source reads a small signed-v2 manifest and
its detached signature from the same repository. These additional metadata
requests likewise contain no scanned content, findings, local paths, or vault
data.

This statement applies to the 0.8.13 personal-core beta and may be revised if future features change its data flows.
