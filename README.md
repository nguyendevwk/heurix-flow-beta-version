# HeurixFlow v0.31.0 [BETA-VERSION]

Low-latency piano auto-player for Sky: Children of the Light.

## 📦 Downloads

| Platform       | File                                     | Size   |
| -------------- | ---------------------------------------- | ------ |
| Linux x86_64   | `HeurixFlow-v0.31.0-linux-x86_64.tar.gz` | ~75 MB |
| Windows x86_64 | `HeurixFlow-v0.31.0-windows-x86_64.zip`  | —      |

## 🚀 Quick Install

### Linux
```bash
tar -xzf HeurixFlow-v0.31.0-linux-x86_64.tar.gz
cd HeurixFlow-v0.31.0
./install.sh
```

### Windows
Run `HeurixFlow-v0.31.0-Setup.exe` → Next → Finish.

## ✨ What's New

- Initial public release
- Low-latency playback engine (Hybrid / Ultra-Spin)
- Piano Roll + Sky Keyboard visual sheet viewer
- Custom keymap editor with presets
- Multi-format parser (JSON, SkySheet, TXT)
- Auto-pause on focus loss (toggle-able)
- Loop / Auto-play / Auto-next modes
- Vietnamese & English UI
- Drag-and-drop song import
- Dark & Light themes

## 🔧 Requirements

- **Linux**: `sudo` access (for evdev UInput kernel module)
- **Windows**: Administrator rights (for keyboard input injection)
- Python 3.12+ (if running from source)

## 🖥️ System Integration

### Linux
After `./install.sh`:
- App appears in system menu as "HeurixFlow"
- No password prompt (sudoers rule configured)
- Uninstall: `sudo rm -rf /opt/HeurixFlow /usr/share/applications/heurixflow.desktop /etc/sudoers.d/heurixflow`

### Windows
After Setup:
- Start Menu shortcut created
- Desktop shortcut (optional)
- Uninstall via Control Panel

## 🐛 Known Issues

- Windows build requires Admin rights for keyboard hooks
- Linux requires `uinput` kernel module: `sudo modprobe uinput`
- Ultra-Spin engine mode uses 100% CPU core (use Hybrid for normal use)

---

*For documentation, see [docs/](docs/)*
