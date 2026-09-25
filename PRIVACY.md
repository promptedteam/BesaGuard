# BesaGuard beta privacy

BesaGuard performs its current scanning and observation workflows locally on the computer. Findings, preferences, development telemetry snapshots, and encrypted holding copies remain under the current user's `%LocalAppData%\BesaGuard` directory.

The application contacts the public `promptedteam/BesaGuard` GitHub repository once after startup to read the small beta update manifest. It contacts GitHub again only if the user presses **Check again** or explicitly downloads an available installer. Those requests are subject to GitHub's own privacy terms and normal network logging. BesaGuard does not upload scanned files, findings, file paths, or holding-vault contents through its update channel.

This statement applies to the 0.8.8 personal-core beta and may be revised if future features change its data flows.
