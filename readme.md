# Dynomite ARM build

This project provides GitHub workflow file to build Netflix's dynomite for
`aarch64` architecture.

Dynomite repo: [Netflix/dynomite](https://github.com/Netflix/dynomite)

# How to:

Navigate to [Actions -> Build on aarch64](https://github.com/ivanpepelko/dynomite-arm-build/actions/workflows/build.yml).
Click on the `Run workflow` button to select workflow
parameters and run.

Parameters:

- git ref: ref from dynomite repo from which the binary will be built
- apply patch: extracted from [https://github.com/Netflix/dynomite/pull/775](https://github.com/Netflix/dynomite/pull/775)
  - build will fail without this at v0.6.22
- debug build: as explained in dynomite readme, off by default
- distro: choose one of available distros to build on, bullseys by default

Built binary can be found after successful run in workflow details artifacts section.
