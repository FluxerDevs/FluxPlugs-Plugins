# Contributing

## Pull requests

- One plugin folder per pull request, one version per pull request.
- Build with the FluxPlugs commit in `toolchain.json` before you push. The `validate` check rebuilds your plugin and fails if the hash in `fluxplug.json` differs.
- Don't commit `dist/`, `releases/` or `node_modules/`.
- Don't edit `CODEOWNERS` or any `release.json`; the publish workflow writes them.
- Changes to `verified.json` go in their own pull request, from a maintainer.

## Review

A new plugin needs a maintainer's approval. An update needs an approval from one of the plugin's owners (`store.json`) or a maintainer. Reviewers check that the README says what the plugin does and sends, that the capabilities are the smallest set that works, and that the source is readable.

## Withdrawing a plugin

Open a pull request that deletes `plugins/<id>/`. Published releases stay on GitHub; the store stops listing the plugin.

## Conduct

The [FluxPlugs code of conduct](https://github.com/FluxerDevs/FluxPlugs/blob/main/CODE_OF_CONDUCT.md) applies here, including to plugin names, icons and READMEs. It also says how to report a problem.
