# LedFx

## Background
_LedFx wants to deliver easy, intuitive and responsive realtime audio analysis and RGB LED strip effect generation to the masses._

## Currently Status
- We're attempting a re-write using Go due to performance issues on low power devices (RPi's) using python, and because a lot of us want to learn Go!

## Who We Are:
 - [Contributors](https://github.com/LedFx/LedFx/blob/master/AUTHORS.rst)

## Auto-fix (autofix.ci)

`.github/workflows/autofix.yml` runs a repository's own `.pre-commit-config.yaml`
with [prek](https://github.com/j178/prek) and lets [autofix.ci](https://autofix.ci)
commit the fixes to the pull request. To opt a repository in, install the
autofix.ci app on it and add `.github/workflows/autofix.yml`:

    name: autofix.ci # must be exactly this
    on:
      pull_request:
    permissions:
      contents: read
    jobs:
      autofix:
        uses: LedFx/.github/.github/workflows/autofix.yml@<commit sha> # main

Run the same hooks locally with `prek run --all-files` (or `prek install`).

## Contributing

- We welcome and embrace all, however we believe that all people should feel safe and be protected within our community. As such, you agree to our [Code of Conduct](https://github.com/LedFx/LedFx/blob/master/CODE_OF_CONDUCT.md) when contributing to our project.
