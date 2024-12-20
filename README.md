# Unofficial qBittorrent build for Windows
![License](https://img.shields.io/github/license/qupo1/qbt_build?cacheSeconds=72000)
![Build](https://img.shields.io/github/actions/workflow/status/qupo1/qbt_build/build.yaml?branch=main&cacheSeconds=3600)
![Release](https://img.shields.io/github/release-date/qupo1/qbt_build?cacheSeconds=7200)
## License
GPLv3
## Features
- Transparent build environment by GitHub Actions
- Built by LLVM (except for OpenSSL) to use latest optimization and security features
- Some compiler security features are used
  - `/guard:cf`
  - `/guard:ehcont`
  - `-fcf-protection=full`
  - `-fstrict-flex-arrays=3`
  - `-ftrivial-auto-var-init=zero`
  - `-fno-delete-null-pointer-checks`
- Targets newer CPU (Intel alderlake or later)
  - `-march=alderlake`
- Uses Full LTO
## Dependencies
- Boost
- libtorrent
- OpenSSL
- Qt
- zlib-ng
