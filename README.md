# Orbit releases

Signed builds of **Orbit**, which connects an Android phone to a Linux desktop.
The source code is private; this repository only hosts release files.

## Android

Download `orbit-<version>.apk` from the latest release and open it on your
phone. After the first install, Orbit updates itself from inside the app.

## Linux desktop (Flatpak)

Add the Orbit repository once; your software centre or `flatpak update` then
keeps it up to date:

```bash
flatpak remote-add --if-not-exists --user flathub https://dl.flathub.org/repo/flathub.flatpakrepo
flatpak remote-add --if-not-exists --user orbit https://rhishikeshjeya-design.github.io/orbit-releases/orbit.flatpakrepo
flatpak install --user orbit dev.orbitapp.Orbit
```

Or download `orbit-<version>.flatpak` from a release and install it with
`flatpak install --user orbit-<version>.flatpak` (no automatic updates).

All releases are signed: the APK with the Orbit release key, the Flatpak
repository and bundles with the Orbit repository GPG key.
