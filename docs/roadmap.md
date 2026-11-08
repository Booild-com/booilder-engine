# Roadmap

> The repository is public before the code lands so the boundaries and roadmap
> can be reviewed. Dates are intentionally omitted until the extraction gate is
> green.

## Phase 1 — Decouple

- [ ] Host adapters for assets, storage, diagnostics, blueprints and logging
- [ ] Shared table UI/HUD extraction (`@booild/vtt-ui`)
- [ ] Table host extraction (`@booild/vtt-client`)
- [ ] Versioned protocol + session token + hidden-information redaction
- [ ] `.booildgame` format, packer, loader and compatibility checks
- [ ] Player API client and offline `LocalTransport`
- [ ] Peer dependencies, compiled CSS, assets and isomorphic fixes

## Phase 2 — Publish

- [ ] Move engine history into this repository
- [ ] npm `0.1.0` with provenance
- [ ] Reference server, playground and fixture packages
- [ ] Engine E2E and fresh visual baselines
- [ ] Docs site + API reference

## Phase 3 — Player clients

- [ ] Standalone web player
- [ ] Electron/Steam client (Windows, Linux/Steam Deck; macOS optional)
- [ ] Capacitor Android client
- [ ] Offline/local play and online lobby

## Phase 4 — Launch

- [ ] Public announcement
- [ ] Good-first-issue set
- [ ] First community release
