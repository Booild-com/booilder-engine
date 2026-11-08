# Booild Engine

> **Status: extraction in progress.** This repository is public early so the
> architecture, package boundaries and roadmap can be reviewed. The engine
> source will land here after the decoupling gate is green; no npm packages are
> published yet.

Booild Engine is the player runtime for the Booild tabletop platform:

- **2D/3D tabletop renderers** (React + Three.js / Canvas 2D)
- **Deterministic rules and physics** shared by client and server
- **Immutable game packages** (`.booildgame`) with assets, blueprints, HUD, rules and localization
- **Player API client** for browsing, installing and playing games
- **Player shells** for web, desktop (Steam) and Android/iOS

## Planned packages

| Package | Purpose |
| :--- | :--- |
| `@booild/types` | Runtime and domain contracts |
| `@booild/blueprints` | Blueprint and HUD schemas |
| `@booild/engine-protocol` | Socket.IO wire contract and version handshake |
| `@booild/game-package` | `.booildgame` format, packer and loader |
| `@booild/engine-adapters` | Host adapter interfaces |
| `@booild/table-logic` | Deterministic rules/state engine |
| `@booild/tabletop-physics` | Deterministic tabletop physics |
| `@booild/engine-client` | Optimistic sync and transports |
| `@booild/player-api` | Public player REST client |
| `@booild/vtt-store` | Shared table state |
| `@booild/vtt-ui` | Shared table UI/HUD |
| `@booild/vtt-client` | Opinionated table host |
| `@booild/vtt-engine` | 3D renderer |
| `@booild/vtt-engine-2d` | 2D renderer |
| `@booild/vtt-assets` | Runtime default assets |

## Architecture

The platform (creator tools, backend, accounts, community, commerce) stays in a
separate proprietary repository. This repository is the **runtime**: it must be
able to build, test and play a game package with no platform code present.

The split is designed around three rules:

1. **Move, don't copy.** Shared source lives in exactly one repository.
2. **The engine never imports platform code.** Host services are injected through adapters.
3. **Games are immutable packages.** Client and server pin the same `releaseId` + `contentHash`.

## Roadmap

- [ ] Decouple the runtime from platform services
- [ ] Publish the first `0.1.0` packages
- [ ] Ship the reference server and playground
- [ ] Ship the web player, Electron/Steam client and Android client
- [ ] Publish the docs site and API reference

See [`docs/roadmap.md`](./docs/roadmap.md) for the detailed phases.

## Contributing

The repository is not accepting engine code until the extraction gate is green.
Architecture feedback, package-boundary issues and documentation suggestions are
welcome now. See [`CONTRIBUTING.md`](./CONTRIBUTING.md).

## License

Apache License 2.0. See [`LICENSE`](./LICENSE) and [`NOTICE`](./NOTICE).
