# MTProxyMax Update Watch

Noise-free watcher for updates that MTProxyMax itself can actually consume.

It watches `SamNet-dev/MTProxyMax/main/mtproxymax.sh` and notifies only when that file changes.
On each real change it reports:
- MTProxyMax `VERSION`
- pinned Telemt `TELEMT_MIN_VERSION` + `TELEMT_COMMIT`
- whether the script changed even if the visible version string did not

Upstream `telemt/telemt` releases alone do **not** trigger notifications.

To receive email from GitHub, watch this repository with **Watch -> Custom -> Releases**.

Baseline at setup:
- MTProxyMax: `1.4.1-LTS`
- Telemt: `3.5.7-4ca7418`
