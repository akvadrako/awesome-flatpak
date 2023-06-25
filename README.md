# Awesome Flatpak

> A curated list of resources for the Flatpak packaging system.

**Contents:** [Remotes](#remotes) | [Tools](#tools) | [Apps](#apps) | [Runtimes](#runtimes) | [Portal](#portal) | [Docs](#docs)

## Quick Reference

| task | example |
| --- | --- |
| Install app | ```flatpak install flatseal``` |
| Show permissions | ```flatpak info --show-permissions org.kde.digikam``` |
| Check size | ```flatpak list --columns=name,size``` | 
| Delete data | ```flatpak remove --delete-data``` |

## Remotes

Official:

- [Flathub](https://flathub.org/repo/flathub.flatpakrepo)
- [Flathub-beta](https://flathub.org/beta-repo/flathub-beta.flatpakrepo)
- [gnome-nightly](https://nightly.gnome.org/gnome-nightly.flatpakrepo)
- [kdeapps](https://distribute.kde.org/kdeapps.flatpakrepo) - [list of apps](https://cgit.kde.org/flatpak-kde-applications.git/tree/)
- *old* [liro](https://repo.liri.io/flatpak/liri.flatpakrepo)

Others:

- [tinywrkb/flatpaks](https://github.com/tinywrkb/flatpaks) - hastily packaged apps, mainly adapted from Arch's AUR
- [winepak](https://dl.winepak.org/repo/winepak.flatpakrepo)
- [firefox](https://firefox-flatpak.mojefedora.cz/)
- [skype](https://github.com/snaggen/skype-app) -  2017

## App Stores

- [Souk](https://gitlab.gnome.org/haecker-felix/souk) - Souk is a flatpak-based App Store, written with GTK4 and Rust.
- [bauh](https://github.com/vinifmor/bauh) - Graphical user interface for installing Linux applications. Supports AppImage, Arch packages (AUR, Pacman), Debian packages, Flatpak, Snap and native Web applications
- [Zorin Store](https://zorin.com/os/) - Zorin OS Store comes pre-loaded with the app catalogs of Flathub, the Snap store, and the Ubuntu & Zorin OS APT repositories, AppImage packages and Windows apps (optionally using Windows App Support, powered by WINE)

## Tools

- [Flatseal](https://flathub.org/apps/details/com.github.tchx84.Flatseal) -  Permissions manager for Flatpak Apps
- [Unsnap](https://github.com/popey/unsnap) - Quickly migrate from using snap packages to flatpaks
- [Sideload](https://github.com/elementary/sideload) - Tool for fast installation .flatpakrefs files, developed Elementary
- *old* rpm2flatpak
- *old* [game-to-flatpak](https://github.com/hadess/flatpak-games) - 2018

## Apps

- [Flathub Wikis](https://github.com/flatpak/flatpak/wiki/Examples)
- [Flathub Search](https://flathub.org/apps)
- [Flathub Beta Search](https://beta.flathub.org/)

## Runtimes

Runtimes provide basic dependencies that can be used by applications. They also provide the environment that applications run in.

### Platforms

- [org.freedesktop.Platform -](https://gitlab.com/freedesktop-sdk/freedesktop-sdk/)
- org.freedesktop.BasePlatform - a smaller runtime
- [org.kde.Platform](https://invent.kde.org/kde/flatpak-kde-runtime) ([Docs](https://community.kde.org/Guidelines_and_HOWTOs/Flatpak))
- [org.gnome.Platform](https://gitlab.gnome.org/GNOME/gnome-build-meta)
- [org.fedora.Platform](https://docs.fedoraproject.org/en-US/flatpak/runtimes/)
- org.fedoraproject.BasePlatform - a smaller runtime
- [org.winepak.Platform](https://github.com/winepak/winepak-sdk-images)

### Base Apps

Base apps contain collections of bundled dependencies which can then be bundled as part of an application. 

- [org.electronjs.Electron2.BaseApp](https://github.com/flathub/org.electronjs.Electron2.BaseApp)
- [io.atom.electron.BaseApp](https://github.com/endlessm/electron-flatpak-base-app) - [example](https://github.com/flathub/electron-sample-app), deprecated

## Portal

Flatpak apps interface with the host system mostly via DBUS calls
to the a daemon [xdg-desktop-portal](https://github.com/flatpak/xdg-desktop-portal) running on the host system.

- [Flathub Wiki Docs](https://github.com/flatpak/flatpak/wiki/Portals)
- [Portal Daemon Docs](https://flatpak.github.io/xdg-desktop-portal/portal-docs.html)

### Backends

To implement most portals, the portal relies on backends like these that provides implementations of the `org.freedesktop.impl.portal.*` interfaces.

- [xdg-desktop-portal-gtk](https://github.com/flatpak/xdg-desktop-portal-gtk) - for GNOME desktops
- [Pantheon XDG Desktop Portals](https://github.com/elementary/portals) - for Elementary desktops
- [xdg-desktop-portal-kde](https://github.com/KDE/xdg-desktop-portal-kde) - for KDE desktops
- [xdg-desktop-portal-lxqt](https://github.com/lxqt/xdg-desktop-portal-lxqt) - for LXQt desktops
- [xdg-desktop-portal-wlr](https://github.com/emersion/xdg-desktop-portal-wlr) - for wlroots-based compositors like Sway
    - supported iterfaces: Request, Session, Screenshot, Screencast

## Docs

- [flatpak dev docs](https://docs.flatpak.org/en/latest/)
- [flatpak wiki](https://github.com/flatpak/flatpak/wiki)
- [flatpak FAQ](https://flatpak.org/faq/)
- [Debian Wiki](https://wiki.debian.org/FlatPak)
- [ArchWiki](https://wiki.archlinux.org/index.php/Flatpak)
- [Fedora](https://docs.fedoraproject.org/en-US/flatpak/)
- [NixOS](https://nixos.org/nixos/manual/index.html#module-services-flatpak)
- [cheatsheet](https://docs.fedoraproject.org/en-US/fedora-silverblue/_attachments/flatpak-print-cheatsheet.pdf)

## News:

- https://flatpak.org/blog-posts/
- https://beta.flathub.org/feeds - Rss feeds
- https://twitter.com/FlathubP - Twitter Account which notify you, when published new or updated flatpak

## Contribute

Contributions welcome. Don't feel the need to put too much effort into it. For now, anything flatpak focused will be accepted and I'll work on the formatting if needed.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, we waive all copyright and
related or neighboring rights to this work.
