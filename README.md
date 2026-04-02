# aghub-bin

AUR binary package for [aghub](https://github.com/AkaraChen/aghub) — One hub for every AI coding agent.

This is an unofficial community-maintained package. The aghub project and its trademarks belong to the upstream developers.

## Install

```bash
paru -S aghub-bin
# or
yay -S aghub-bin
```

## Links

- Upstream: [AkaraChen/aghub](https://github.com/AkaraChen/aghub)
- AUR: [aghub-bin](https://aur.archlinux.org/packages/aghub-bin)

## Reporting Issues

- **Application bugs** (UI glitches, agent config errors, etc.) → report to [upstream](https://github.com/AkaraChen/aghub/issues)
- **Packaging issues** (install failures, .desktop file, PKGBUILD/checksum errors) → report [here](https://github.com/losslauralin/aur-aghub-bin/issues)

## Troubleshooting

### Wayland users (blank window / rendering issues)

aghub uses WebKit2GTK which may not render correctly under Wayland. The `.desktop` entry already forces X11 mode. If launching from terminal:

```bash
GDK_BACKEND=x11 WEBKIT_DISABLE_DMABUF_RENDERER=1 aghub
```
