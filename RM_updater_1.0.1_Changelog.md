# Changelog – RM_updater_1.0.0

**Release Date:** [Insert release date here]

## ✨ Features
- **Graphical User Interface (GUI)** built with PyQt6 for a clean and user-friendly update process.
- **Dynamic folder selection**: users can select the target directory where the RetMan application should be updated.
- **Live progress bar** indicating download completion percentage for real-time feedback.
- **Automatic ZIP extraction**: the updater downloads and unpacks the latest `RetMan.zip` release.
- **Executable launcher**: automatically runs the newly downloaded `RetMan.exe` upon successful update.
- **Clean directory management**: previous files are removed to ensure a clean installation environment, except essential ones like `RetMan.exe` and `login.dist`.

## 🖼 UI Enhancements
- Embedded **custom logo (`logo.png`)** displayed at the top of the window.
- Custom **window icon (`icon.ico`)** for professional branding.
- Polished layout with margins, spacing, and font adjustments.

## 🛠 Internal Improvements
- Uses `resource_path()` to ensure compatibility with `PyInstaller`'s frozen environment, enabling proper loading of image and icon files.
- Handles download and extraction in a separate thread to keep the GUI responsive.
- Error handling through `QMessageBox` to notify users of issues during the update or launch phases.
