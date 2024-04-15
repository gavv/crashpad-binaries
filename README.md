# crashpad-binaries [![build](https://github.com/gavv/crashpad-binaries/actions/workflows/build.yml/badge.svg)](https://github.com/gavv/crashpad-binaries/actions/workflows/build.yml)

Prebuilt [Google Crashpad](https://chromium.googlesource.com/crashpad/crashpad) binaries for Windows (x64 MSVC) and macOS (universal binaries).

For Linux, instead of binaries there is a branch with fully fetched crashpad source code with all dependencies and build tools, suitable for offline build on 64-bit Linux machine.

Binaries are built and published automatically using Github Actions. You can either use binaries from this repo, or fork the repo and configure your own build, so that you can completely trust the build results.

Branch    | Description
--------- | ------
[`main`](https://github.com/gavv/crashpad-binaries) | build script and github actions config
[`macos`](https://github.com/gavv/crashpad-binaries/tree/macos) | macOS binaries (suitable both for Intel and M1)
[`VS2019_MD`](https://github.com/gavv/crashpad-binaries/tree/VS2019_MD) | Windows binaries (Visual Studio 2019, MD runtime)
[`VS2019_MDd`](https://github.com/gavv/crashpad-binaries/tree/VS2019_MDd) | Windows binaries (Visual Studio 2019, MDd runtime)
[`linux_source`](https://github.com/gavv/crashpad-binaries/tree/source) | crashpad source code prepared for offline linux64 build

The list of available versions is [available here](https://github.com/gavv/crashpad-binaries/tags).

The binaries are built using [depot_tools](https://www.chromium.org/developers/how-tos/install-depot-tools/). On Windows Visual Studio 2019 is used. There are separate builds for `/MD` and `/MDd` runtime, published as different branches and tags. You can find exact build options [here](https://github.com/gavv/crashpad-binaries/blob/main/.github/workflows/build.yml).
