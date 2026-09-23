# AMI Chat AppImage

Linux AppImage that opens `aitools.ptit.edu.vn/chat/` as a
standalone desktop app — using Chrome/Chromium's `--app` mode, fixed at a
mobile-sized window, launchable from a desktop icon.

Doesn't bundle a browser — it still requires Chrome or Chromium to
already be installed on the system; the AppImage just launches it with
the right flags.

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/f5a0d7df-3229-43df-b05d-a4003ebd8a11" />


## Run

```bash
chmod +x AMI-Chat.AppImage
./AMI-Chat.AppImage
```

## Requirements

- Chrome or Chromium installed (`google-chrome-stable`, `google-chrome`,
  `chromium-browser`, or `chromium`)
- `libfuse2` to run AppImages on some newer Debian/Mint releases
  (if it fails, run `./AMI-Chat.AppImage --appimage-extract-and-run`)

## License

MIT — see [LICENSE](LICENSE).
