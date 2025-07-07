# 🖥️ ToDo Desktop App (WebView Wrapper)

This project wraps the existing Django-based ToDo web application (`https://todo-list-up2x.onrender.com`) into a standalone **desktop app (.exe)** using **pywebview** and **PyInstaller**.

---

## 📦 Requirements

Install these packages in a virtual environment:

```bash
pip install pywebview
pip install pyinstaller


---

## 📁 File Structure

```
TodoDesktop/
├── TodoApp.py           # Python file to load the web app
├── icon.ico             # (Optional) App icon
├── dist/                # Final .exe output after packaging
└── build/               # PyInstaller build files
```

---

## 📝 Python Code (TodoApp.py)

```python
import webview

# Replace with your actual Render URL
URL = "https://todo-list-up2x.onrender.com"

webview.create_window("ToDo App", URL)
webview.start()
```

---

## 🚀 Run the Desktop App Locally

```bash
python TodoApp.py
```

> This will open your hosted Django app in a native desktop window.

---

## 🧱 Convert to .exe File

Run the following command:

```bash
pyinstaller --noconfirm --onefile --windowed --clean --icon=icon.ico TodoApp.py
```

### Flags Explained:

* `--noconfirm`: Overwrites output without asking.
* `--onefile`: Combines into a single `.exe`.
* `--windowed`: Hides console window.
* `--clean`: Removes previous build cache.
* `--icon=icon.ico`: Optional, sets window icon.

---

## 📂 Output

After building, check the `dist/` folder:

```
dist/
└── TodoApp.exe
```

Double-click `TodoApp.exe` to launch the desktop app.

---

## ⚠️ Important Notes

* The app **requires an internet connection** to access the hosted Django website.
* Antivirus software may **falsely flag** the `.exe` as malicious. To reduce false positives:

  * Build on a clean, trusted environment.
  * Digitally sign the executable.
  * Use reputable tools like **Nuitka** for more secure builds.

---

## 🧰 Tools Used

* 🐍 Python 3.x
* 🌐 [pywebview](https://pywebview.flowrl.com/)
* 📦 [PyInstaller](https://pyinstaller.org/)
* 🎨 (Optional) icon.ico for branding

---

## 👨‍💻 Created by

**Ponnarasu A**

---

```

Let me know if you want a `README.md` for the **React Native mobile version** or **Nuitka-based secure build** as well.
```
