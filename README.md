# AMI Chat AppImage

A personal Linux AppImage that opens `aitools.ptit.edu.vn/chat/` as a
standalone desktop app — using Chrome/Chromium's `--app` mode, fixed at a
mobile-sized window, launchable from a desktop icon.

Doesn't bundle a browser — it still requires Chrome or Chromium to
already be installed on the system; the AppImage just launches it with
the right flags.

## Run

```bash
chmod +x AMI-Chat.AppImage
./AMI-Chat.AppImage
```

## Customize

The window URL and size are baked into this build. If you want to change
them, you'd need to edit `AppRun` inside the AppDir and repackage with
`appimagetool` — happy to walk through that if needed.

## Requirements

- Chrome or Chromium installed (`google-chrome-stable`, `google-chrome`,
  `chromium-browser`, or `chromium`)
- `libfuse2` to run AppImages on some newer Debian/Mint releases
  (if it fails, run `./AMI-Chat.AppImage --appimage-extract-and-run`)

## License

MIT — see [LICENSE](LICENSE).
