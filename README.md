<div align="center">

<img width="100%" src="assets/readme-hero.svg" alt="Leviathan Integrations">

<br>

<img src="https://img.shields.io/badge/status-active%20development-06131d?style=flat-square" alt="Active development">
<img src="https://img.shields.io/badge/scope-public%20integrations-06131d?style=flat-square" alt="Public integrations">
<img src="https://img.shields.io/badge/license-Apache--2.0-06131d?style=flat-square" alt="Apache 2.0">

**Public integration patterns for connecting Leviathan with supported platforms and services.**

[Guide](GUIDE.md) · [API Docs](https://github.com/Lapinite/Leviathan-API-Docs) · [SDK](https://github.com/Lapinite/Leviathan-SDK) · [Examples](https://github.com/Lapinite/Leviathan-Examples) · [Security](SECURITY.md)

</div>

## Integration map

<table width="100%">
<tr>
<td width="33%" valign="top"><strong>Minecraft</strong><br><sub>Plugin integrations · server events · compatibility adapters · public server interfaces</sub></td>
<td width="33%" valign="top"><strong>Community & Messaging</strong><br><sub>Discord · notifications · supported event bridges · moderation-facing integrations</sub></td>
<td width="33%" valign="top"><strong>Platform</strong><br><sub>Webhooks · public APIs · third-party services · lifecycle and permission boundaries</sub></td>
</tr>
</table>

## Scope

Integration work may include:

- Minecraft plugin integrations
- Discord integrations
- webhook producers and consumers
- public API integrations
- server event bridges
- supported third-party service adapters
- compatibility and lifecycle helpers

Only integrations intentionally intended for public use should be published here.

## Integration lifecycle

```text
External System
      ↓
Supported Adapter / Plugin / Webhook
      ↓
Permission + Authentication Boundary
      ↓
Public Leviathan Interface
      ↓
Documented Result / Event
```

Each integration should make its authentication, permissions, configuration, supported versions, failure behavior, and data boundaries clear.

## Navigation

- [Minecraft plugins](GUIDE.md#minecraft-plugins)
- [Discord](GUIDE.md#discord)
- [Webhooks](GUIDE.md#webhooks)
- [Third-party services](GUIDE.md#third-party-services)
- [Permissions](GUIDE.md#permissions)
- [Authentication boundaries](GUIDE.md#authentication-boundaries)
- [Lifecycle](GUIDE.md#lifecycle)
- [Support](GUIDE.md#support)

## Security boundaries

Integrations must never contain real bot tokens, webhook credentials, API secrets, private keys, database credentials, personal information, internal infrastructure addresses, or private administrative endpoints.

Configuration examples should use placeholders or environment-variable names. Logging should avoid exposing secrets or sensitive user data.

## Compatibility

Compatibility information will be documented per integration as implementations become available. Planned integrations must not be represented as production-ready before they have been tested and intentionally released.

## Related repositories

| Repository | Role |
| --- | --- |
| [Leviathan API Docs](https://github.com/Lapinite/Leviathan-API-Docs) | Public interface contracts |
| [Leviathan SDK](https://github.com/Lapinite/Leviathan-SDK) | Developer helpers |
| [Leviathan Examples](https://github.com/Lapinite/Leviathan-Examples) | Small integration examples |
| [Leviathan Server Tools](https://github.com/Lapinite/Leviathan-Server-Tools) | Minecraft server tooling |
| [Leviathan Docs](https://github.com/Lapinite/Leviathan-Docs) | Ecosystem documentation |

## License

This repository uses the Apache License 2.0. See [LICENSE](LICENSE).
