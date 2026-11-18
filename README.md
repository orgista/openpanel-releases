<p align="center">
  <img alt="OpenPanel icon" src="docs/assets/icon.png" width="96">
</p>

<h1 align="center">OpenPanel</h1>

<h3 align="center">Kiosk launcher for Android tablets, Google TV and XR headsets</h3>

<p align="center">
  <a href="https://github.com/orgista/openpanel-releases/releases">Download</a> ·
  <a href="https://orgista.com/products/openpanel">orgista.com</a>
</p>

OpenPanel is a kiosk launcher for Android tablets, Google TV and XR headsets.
It shows an approved set of apps, YouTube videos and channels, and an offline
books and audio shelf, and keeps the device on that set.

This repository only holds builds. Download the APK from
[Releases](https://github.com/orgista/openpanel-releases/releases); each release
has its install steps and SHA-256 checksum.

The source code will be published when OpenPanel launches.

## Releases

[![Latest release](https://img.shields.io/github/v/release/orgista/openpanel-releases?include_prereleases&sort=semver)](https://github.com/orgista/openpanel-releases/releases)
[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/orgista/openpanel-releases/badge)](https://scorecard.dev/viewer/?uri=github.com/orgista/openpanel-releases)

Downloads live on the [Releases page](https://github.com/orgista/openpanel-releases/releases): the signed APK (`openpanel-X.Y.Z.apk`).
The APK is built and signed on our build Mac from the private OpenPanel source and published there. Source, CHANGELOG and the build scripts live in the private OpenPanel repo; its releases are published here.

- **Versions** follow [Semantic Versioning](https://semver.org/): `vMAJOR.MINOR.PATCH`. A version with a
  suffix (`v1.4.0-beta.1`) is a pre-release and is marked as one.
- **Cadence:** we ship when a change is ready, and at least one maintenance release a month while the project
  is in active development. Security fixes ship within 7 days of a confirmed report.
- **Every release** has release notes taken from the source repo's CHANGELOG, a `SHA256SUMS` checksum file and a GitHub attestation for every file.
- **Support:** only the latest release gets fixes. Please update before reporting a bug.

Check a download before installing it:

```bash
shasum -a 256 -c SHA256SUMS --ignore-missing
gh attestation verify openpanel-1.1.64.apk --repo orgista/openpanel-releases
```

## License

MIT.
