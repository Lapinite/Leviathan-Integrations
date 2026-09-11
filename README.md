# Leviathan Integrations

Official public integrations for connecting supported Leviathan interfaces with Minecraft server software, Discord, webhooks, and other supported platforms.

## Navigation

See the [public guide](GUIDE.md) for availability, usage boundaries, and topic-by-topic documentation. Read [SECURITY.md](SECURITY.md) before reporting a security issue.

- [Minecraft plugins](GUIDE.md#minecraft-plugins)
- [Discord](GUIDE.md#discord)
- [Webhooks](GUIDE.md#webhooks)
- [Third-party services](GUIDE.md#third-party-services)
- [Permissions](GUIDE.md#permissions)
- [Authentication boundaries](GUIDE.md#authentication-boundaries)
- [Lifecycle](GUIDE.md#lifecycle)
- [Support](GUIDE.md#support)

## Scope

Integration work may include:

- Minecraft plugin integrations
- Discord integrations
- Webhook producers and consumers
- Public API integrations
- Server event bridges
- Supported third-party service adapters

Only integrations intended for public use should be published here.

## Security

Integrations must never contain real bot tokens, webhook credentials, API secrets, private keys, database credentials, personal information, or private infrastructure endpoints.

Configuration examples should use placeholders or environment-variable names rather than real credentials.

## Compatibility

Compatibility information will be documented per integration as implementations become available. Planned integrations should not be represented as production-ready before they have been tested and released.

## Related repositories

- [Leviathan API Docs](https://github.com/Lapinite/Leviathan-API-Docs)
- [Leviathan SDK](https://github.com/Lapinite/Leviathan-SDK)
- [Leviathan Examples](https://github.com/Lapinite/Leviathan-Examples)
- [Leviathan Server Tools](https://github.com/Lapinite/Leviathan-Server-Tools)

## License

This repository currently uses the Apache License 2.0. See [LICENSE](LICENSE).
