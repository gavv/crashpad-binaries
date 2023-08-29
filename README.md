# crashpad-win64 [![build](https://github.com/gavv/crashpad-win64/actions/workflows/build.yml/badge.svg)](https://github.com/gavv/crashpad-win64/actions/workflows/build.yml)

Prebuilt [Google Crashpad](https://chromium.googlesource.com/crashpad/crashpad) binaries for Windows (x64 MSVC) and macOS (universal binaries).

Branch    | Description
--------- | ------
[`main`](https://github.com/gavv/crashpad-win64) | build script and github actions config
[`macos`](https://github.com/gavv/crashpad-win64/tree/macos) | macOS binaries (suitable both for Intel and M1)
[`VS2019_MD`](https://github.com/gavv/crashpad-win64/tree/VS2019_MD) | Windows binaries (Visual Studio 2019, MD runtime)
[`VS2019_MDd`](https://github.com/gavv/crashpad-win64/tree/VS2019_MDd) | Windows binaries (Visual Studio 2019, MDd runtime)

The list of available versions is [available here](https://github.com/gavv/crashpad-win64/tags).

The binaries are built using [depot_tools](https://www.chromium.org/developers/how-tos/install-depot-tools/). On Windows Visual Studio 2019 is used. There are separate builds for `/MD` and `/MDd` runtime, published as different branches and tags. You can find exact build options [here](https://github.com/gavv/crashpad-win64/blob/main/.github/workflows/build.yml).
