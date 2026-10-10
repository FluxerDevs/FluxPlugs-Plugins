# FluxPlugs community plugins

Plugins for the [Fluxer](https://fluxer.app) desktop app, built on [FluxPlugs](https://fluxer.plus). Everything merged here is built, scanned and published to the [plugin store](https://fluxer.plus/plugins/).

## Publish a plugin

The full guide is [Publish to the plugin store](https://fluxer.plus/develop/publishing/store/). In short:

1. Build your plugin with the FluxPlugs commit pinned in `toolchain.json`, so the hash in `fluxplug.json` matches what the workflow rebuilds.
2. Add `plugins/<id>/` with `fluxplug.json`, `store.json`, `README.md` and `src/`, plus an optional `icon.png` and `CHANGELOG.md`.
3. Open a pull request that changes that one folder. The `validate` check tells you what to fix. While FluxPlugs is in its private beta, that check can only run on branches of this repository, not on forks, because it needs a token for the FluxPlugs code; a maintainer runs it for you.
4. After the merge, `publish` creates the release `<id>-v<version>`, writes `plugins/<id>/release.json`, and the store updates a few minutes later.

To update, raise `version` and open another pull request. Owners listed in `store.json` review changes to their plugin.

## Reviewed

Every published plugin is Listed. A maintainer who has read a version's code adds its hash to `verified.json`, and the store shows that version as Reviewed. Ask for a review with a **Verification request** issue. Reviewed means reviewed for malware; it is not an endorsement, and Fluxer may still act against accounts that use automation.

## Report a plugin

Open a **Plugin report** issue. For anything that looks like malware, write to the maintainers listed in `maintainers.json` directly as well.

## License

The workflows, templates and lists in this repository are under the [MIT license](LICENSE). Each plugin is under the license named in its `store.json`.
