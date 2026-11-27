# Embedded Termux integration for DJALIMEN

## Target architectures

| Termux architecture | Android ABI |
| --- | --- |
| aarch64 | arm64-v8a |
| arm | armeabi-v7a |
| x86_64 | x86_64 |

## Bootstrap identity

The bootstrap must be compiled for the Android application package ID
`com.djalimen.manager`, so its prefix is
`/data/data/com.djalimen.manager/files/usr`. An official prebuilt
`com.termux` bootstrap must not be extracted into this application: package
scripts and binaries are built with a package-specific prefix.

## Bootstrap build

The manual GitHub Actions workflow
`.github/workflows/build-termux-bootstrap.yml` builds the three bootstrap
archives from the Termux package sources using the documented
`agnostic-apollo/termux-packages` `infra-improvs` bootstrap builder.
Each architecture is built separately and uploaded as an artifact.

## Runtime integration status

This workflow is the bootstrap-build foundation only. The app must still
vendor/import the matching Termux `terminal-view`, `terminal-emulator`,
and `termux-shared` libraries, install the matching bootstrap on first
launch, configure the shell environment and lifecycle, and expose the
terminal screen from Home. Do not advertise the embedded terminal as usable
until those runtime steps and device tests are complete.

## Licensing

Termux source code and package sources remain subject to their respective
upstream licenses and copyright notices. Keep upstream license files and
attribution with any redistributed code or bootstrap components.
