# 01. Linux distributions

_Video length: 7 min | Status: done_

## Summary

A Linux distribution ("distro") is the Linux kernel plus everything built around it, i.e. tools, apps, defaults, and user experience. Every distro shares the same kernel. What differs is the packaging and choices layered on top. Red Hat's family has three tiers: Fedora (upstream, cutting-edge, risky), CentOS Stream (midstream, rolling preview of the next RHEL release), and RHEL itself (downstream, stable, tested, enterprise-grade). Features flow from Fedora → CentOS Stream → RHEL over time.

## Key takeaways

- All Red Hat-family distros (Fedora, CentOS Stream, RHEL) use the same kernel and the same RPM package manager, different from Ubuntu/Debian's Apt/DPKG, and the two aren't compatible.

- RHEL follows the File Hierarchy Standard (FHS), so `/etc`, `/usr`, `/var` etc. are where you'd expect. Not all distros stick to this strictly.

- Red Hat both uses and contributes back to open source (systemd, KVM, Tuned all started at Red Hat).

- RHEL isn't just for big enterprises. There's a free developer subscription (up to 16 systems, full updates, self-service support) for non-production/learning use.

- RHEL releases a new major version every 3 years. Upgrades use a tool called Leap.

- Support has 3 phases: full support (5 yrs, features + fixes + security), maintenance support (next 5 yrs, security only), and an optional extended update support add-on after that.

## New terms

| Term | Meaning |
|------|---------|
| Distro | A complete OS built around the Linux kernel, with its own tools, packaging, and defaults |
| Kernel | The core code shared by every Linux distribution |
| Upstream / midstream / downstream | Fedora = upstream (newest, most experimental); CentOS Stream = midstream (preview of next RHEL); RHEL = downstream (stable, released) |
| RPM | Red Hat Package Manager. How RHEL/Fedora/CentOS Stream install, update, and remove software (since 1997) |
| FHS | File Hierarchy Standard. The standard layout of directories like `/etc`, `/usr`, `/var` that RHEL follows |
| Leapp | Red Hat's tool for upgrading between major RHEL versions |
| Extended Update Support (EUS) | An add-on giving select security patches after full + maintenance support end |

## Questions to look into later

- What exactly changes for me day-to-day if I pick RHEL over CentOS Stream for a home lab, given both are free to use in some form?

- What's actually in the free developer subscription's "self-service support"? Is that just docs/forums, or something more?
