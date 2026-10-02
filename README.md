# MTProxyMax Update Watch

Noise-free watcher for target updates: a new MTProxyMax version and/or a new Telemt version pinned by MTProxyMax.

It watches `SamNet-dev/MTProxyMax/main/mtproxymax.sh`, but sends a Release notification only when `VERSION`, `TELEMT_MIN_VERSION`, or `TELEMT_COMMIT` changes.
On each target update it reports:
- MTProxyMax `VERSION`
- pinned Telemt `TELEMT_MIN_VERSION` + `TELEMT_COMMIT`
Upstream `telemt/telemt` releases alone do **not** trigger notifications. Script-only edits with the same MTProxyMax version and the same Telemt pin are recorded silently and do **not** trigger notifications.

To receive email from GitHub, watch this repository with **Watch -> Custom -> Releases**.

Baseline at setup:
- MTProxyMax: `1.4.1-LTS`
- Telemt: `3.5.7-4ca7418`
