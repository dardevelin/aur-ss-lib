# SS_Lib AUR Package

This repository contains the AUR (Arch User Repository) package for [SS_Lib](https://github.com/dardevelin/ss_lib) - a lightweight signal-slot library for C.

## Installation

### From AUR (recommended)
```bash
yay -S ss-lib
# or
paru -S ss-lib
```

### Manual Build
```bash
git clone https://github.com/dardevelin/aur-ss-lib.git
cd aur-ss-lib
makepkg -si
```

## Package Contents

- **ss-lib**: Latest stable release from GitHub releases
- Headers installed to `/usr/include/ss_lib/`
- Library installed to `/usr/lib/libss_lib.a`
- Single header version at `/usr/include/ss_lib_single.h`
- pkg-config file for easy linking

## Usage After Installation

```bash
# Compile with pkg-config
gcc your_app.c $(pkg-config --cflags --libs ss_lib) -o your_app

# Or manually
gcc your_app.c -I/usr/include/ss_lib -lss_lib -o your_app
```

## Package Information

- **Maintainer**: dardevelin
- **Architecture**: i686, x86_64, armv7h, aarch64
- **License**: MIT
- **Dependencies**: None (zero dependencies)
- **Build Dependencies**: gcc, make

## Updates

This package tracks the latest stable releases from the main repository. The PKGBUILD is updated automatically or manually for each new release.

For the latest development version, see the upstream repository: https://github.com/dardevelin/ss_lib

## Issues

- For package-specific issues (build failures, installation problems): Open issues here
- For library bugs or feature requests: Open issues at https://github.com/dardevelin/ss_lib
EOF < /dev/null