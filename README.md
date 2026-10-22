# Claude Desktop Flatpak (io.github.dewzor.ClaudeDesktop)

**Archived on October 22, 2026.** This Flatpak is no longer maintained. The Flathub submission was closed, and the manifest still pins Claude Desktop 1.40609.0 from August 2026. On Fedora, use the native RPM instead: https://github.com/dewzor/claude-desktop-fedora

Flatpak manifest for Claude Desktop on Linux, built from Anthropic's official .deb via extra-data. Nothing proprietary is redistributed; Flatpak downloads the package on your machine at install time.

Build and install locally:

```
git clone https://github.com/dewzor/ClaudeDesktop
cd ClaudeDesktop
flatpak-builder --user --install --force-clean build-dir io.github.dewzor.ClaudeDesktop.yaml
flatpak run io.github.dewzor.ClaudeDesktop
```

Claude Code inside the Flatpak runs on the host through the Flatpak portal (host-spawn), so it sees your real git, node, python and project tools. The RPM build for Fedora, the COPR package and the project docs live at https://github.com/dewzor/claude-desktop-fedora.
