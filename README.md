# UniVex Releases (development)

Private development builds of **UniVex Hub** and the **UniVex Engine**, for testing before a public
release. Nothing here is meant for users; public releases are published separately.

## What a release holds

| Tag                   | Files                                                                      |
| --------------------- | -------------------------------------------------------------------------- |
| `v<version>`          | `univex-engine-<version>-<platform>.uvpackage` and its `.sha256`, per platform |
| `hub-v<version>`      | `UniVexHubSetup-<version>-<platform>` installers and their `.sha256`        |

Tags ending in `-beta` are marked as prereleases.

## Testing a build

1. From the newest `hub-v…` release, download and run the Hub installer for your system.
2. From the newest `v…` release, download the `.uvpackage` for your system together with its
   `.sha256` file, and keep both in the same folder.
3. In UniVex Hub, open **Engines → Import package...** and choose the `.uvpackage`. The Hub checks it
   against the `.sha256` file beside it before installing.

The Hub does not read this repository on its own (it is private), which is why development engines
are imported by hand.
