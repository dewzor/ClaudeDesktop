# Claude Desktop Flatpak (io.github.dewzor.ClaudeDesktop)

Flatpak manifest for Claude Desktop on Linux, built from Anthropic's official .deb via extra-data. Nothing proprietary is redistributed; Flatpak downloads the package on your machine at install time.

Status: submitted to Flathub, https://github.com/flathub/flathub/pull/9971. While the review runs, this repo is where the manifest is edited. After the merge, the manifest lives in Flathub's own repo for this app and this repo stays as the app-id home and screenshot host.

Build and install locally:

```
git clone https://github.com/dewzor/ClaudeDesktop
cd ClaudeDesktop
flatpak-builder --user --install --force-clean build-dir io.github.dewzor.ClaudeDesktop.yaml
flatpak run io.github.dewzor.ClaudeDesktop
```

Claude Code inside the Flatpak runs on the host through the Flatpak portal (host-spawn), so it sees your real git, node, python and project tools. The RPM build for Fedora, the COPR package and the project docs live at https://github.com/dewzor/claude-desktop-fedora.
