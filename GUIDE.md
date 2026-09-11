# Integration guide

[Integration overview](README.md)

**Status: planned adapters.** The repository currently provides documentation and licensing, with no released adapter implementation.

## Minecraft plugins

A future plugin must specify Minecraft version, server software, Java version, installation steps, commands, permissions, and removal steps. No Paper, Spigot, Bukkit, or other server compatibility is claimed without a tested release.

## Discord

Discord integration is planned. A future adapter should request only permissions needed for documented functions. Keep bot credentials in private runtime configuration. Never place a real webhook URL in source, examples, logs, screenshots, or public issues.

## Webhooks

Producers and consumers require a released contract covering event schemas, authentication, replay handling, retries, and duplicate deliveries. No public webhook endpoint or signing scheme is specified yet.

## Third-party services

No supported-service matrix is currently published. Each adapter must identify its provider, supported versions, required permissions, licensing, and applicable service terms. A product mentioned as an integration area is not a compatibility guarantee.

## Permissions

Document minimum permissions per operation. Separate administrative setup from ordinary operation. Avoid asking users for broad server or account permissions when a narrower permission is sufficient.

## Authentication boundaries

The integration authenticates only to its intended service. A Minecraft account token must not become a generic integration credential. Server-side secrets belong in private runtime storage; public clients cannot safely contain confidential secrets. Never reuse the launcher's application registration.

## Lifecycle

1. Confirm that the adapter and service contract are publicly released.
2. Review versions, permissions, and installation instructions.
3. Configure credentials outside source control.
4. Validate behavior in an authorized test environment without real data in public fixtures.
5. Update using release notes and compatibility guidance.
6. On removal, revoke credentials and permissions and delete private runtime data as appropriate.

## Support

Report ordinary issues with adapter version, server/runtime version, and sanitized reproduction steps. Follow [SECURITY.md](SECURITY.md) for security concerns.
