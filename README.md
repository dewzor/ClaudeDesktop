# Claude Desktop Flatpak (io.github.dewzor.ClaudeDesktop)

Flatpak manifest for Claude Desktop on Linux, built from Anthropic's official .deb via extra-data. Nothing proprietary is redistributed; the package downloads at install time.

This repo exists to back the Flathub app ID. Development, docs, the RPM/COPR path and the Fedora build script live at https://github.com/dewzor/claude-desktop-fedora (see its `flatpak/` directory and README).

Build locally:

```
flatpak-builder --user --install --force-clean build-dir io.github.dewzor.ClaudeDesktop.yaml
flatpak run io.github.dewzor.ClaudeDesktop
```
