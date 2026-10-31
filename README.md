# Contrail resources

The scriptlet and redirect resources (`resources.json`) that Contrail for iPhone and iPad uses for
ad and tracker blocking. Each release holds one `resources.json`, built by Contrail's CI from pinned,
unmodified upstream files. The app downloads it and uses it only when its SHA-256 matches the
digest built into the app.

Contrail's own code is not in this repository.

## Sources and licences

`resources.json` is an aggregate of two upstream works, each under its own licence:

- uBlock Origin's scriptlets and redirect resources, from
  [gorhill/uBlock](https://github.com/gorhill/uBlock), GPL-3.0 ([LICENSES/GPL-3.0.txt](LICENSES/GPL-3.0.txt)).
- Brave's resources, from [brave/adblock-resources](https://github.com/brave/adblock-resources),
  MPL-2.0 ([LICENSES/MPL-2.0.txt](LICENSES/MPL-2.0.txt)).

Each release's notes name the exact upstream commits it was built from. The resources are
JavaScript and are included as source; the upstream repositories at those commits hold the
originals.
