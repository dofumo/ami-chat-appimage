# AMI Chat AppImage

A personal Linux AppImage that opens `aitools.ptit.edu.vn/chat/` as a
standalone desktop app — using Chrome/Chromium's `--app` mode, fixed at a
mobile-sized window, launchable from a desktop icon.

Doesn't bundle a browser — it still requires Chrome or Chromium to
already be installed on the system; the AppImage just launches it with
the right flags.

## Build

```bash
cd appimage
./build.sh
```

The script downloads `appimagetool` (requires internet) and packages
`AMI-Chat.AppDir` into `AMI-Chat.AppImage`.

## Run

```bash
./AMI-Chat.AppImage
```

## Customize

Edit `URL`, `WIDTH`, `HEIGHT` in `AMI-Chat.AppDir/AppRun`, then rebuild.

To change the icon, replace `AMI-Chat.AppDir/ami-icon.png` and `.DirIcon`
with another square PNG, then rebuild.

## Requirements

- Chrome or Chromium installed (`google-chrome-stable`, `google-chrome`,
  `chromium-browser`, or `chromium`)
- `libfuse2` to run AppImages on some newer Debian/Mint releases
  (if it fails, run `./AMI-Chat.AppImage --appimage-extract-and-run`)

## License

MIT — see [LICENSE](LICENSE).
