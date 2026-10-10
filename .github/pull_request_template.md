## Plugin

<!-- The id, and whether this is a new plugin or a new version. -->

## What changed

<!-- For an update: what users will notice. For a new plugin: what it does and what it sends where. -->

## Checklist

- [ ] The folder `plugins/<id>/` is named after the manifest's `id`.
- [ ] I built with the FluxPlugs commit in `toolchain.json` and committed the resulting `fluxplug.json`.
- [ ] `version` is higher than the published one (new plugin: any semantic version).
- [ ] `README.md` is written for users and says what the plugin sends where.
- [ ] `store.json` lists every owner, and I am one of them.
- [ ] No `dist/`, `releases/` or `node_modules/` are committed.
