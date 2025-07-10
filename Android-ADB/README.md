# ADB Commands Guide for Android (Windows & Linux)

This guide provides a comprehensive list of ADB (Android Debug Bridge) commands with usage instructions for both **Windows** and **Linux** platforms.

---

## 📦 Installation
### Linux:
```bash
sudo apt update
sudo apt install android-tools-adb android-tools-fastboot
```

### Windows:
1. Download [Platform Tools](https://developer.android.com/studio/releases/platform-tools).
2. Extract the ZIP.
3. Open CMD or PowerShell in the folder.
4. Use commands with `./adb` prefix:
```bash
./adb devices
```
![image](https://github.com/user-attachments/assets/1d246d0f-d39f-4a8a-88a1-9d747c8148aa)

---

## 🔧 Common ADB Commands
| Command                                | Description                          | Linux              | Windows             |
|----------------------------------------|--------------------------------------|--------------------|---------------------|
| List devices                           | Check connected devices              | `adb devices`      | `./adb devices`     |
| Start shell                            | Launch ADB shell                     | `adb shell`        | `./adb shell`       |
| Reboot device                          | Restart device                       | `adb reboot`       | `./adb reboot`      |
| Install APK                            | Install application                  | `adb install app.apk` | `./adb install app.apk` |
| Uninstall app                          | Remove application                   | `adb uninstall <package>` | `./adb uninstall <package>` |

---

## 🗂 File Management
| Task            | Linux Example                  | Windows Example                   |
|-----------------|--------------------------------|-----------------------------------|
| Push file       | `adb push file.txt /sdcard/`   | `./adb push file.txt /sdcard/`    |
| Pull file       | `adb pull /sdcard/file.txt`    | `./adb pull /sdcard/file.txt`     |

---

## 📺 Screen Capture & Recording
| Task           | Linux                          | Windows                          |
|----------------|----------------------------------|----------------------------------|
| Screenshot     | `adb shell screencap /sdcard/screen.png` | `./adb shell screencap /sdcard/screen.png` |
| Screen Record  | `adb shell screenrecord /sdcard/rec.mp4` | `./adb shell screenrecord /sdcard/rec.mp4` |

---

## 🎮 Input Simulation
| Task                | Linux Command                        | Windows Command                     |
|---------------------|---------------------------------------|-------------------------------------|
| Tap screen          | `adb shell input tap 500 700`        | `./adb shell input tap 500 700`     |
| Input text          | `adb shell input text 'Hello'`       | `./adb shell input text "Hello"`    |

---

## 🌐 Wireless ADB
1. Connect via USB and enable TCP/IP:
```bash
adb tcpip 5555          # Linux
./adb tcpip 5555        # Windows
```

2. Get device IP and connect:
```bash
adb connect <ip>:5555   # Linux
./adb connect <ip>:5555 # Windows
```

---

## 🧠 Notes
- Always enable **Developer Options** > **USB Debugging**.
- On Windows, always prefix commands with `./adb` if you're in the platform-tools folder.
- Use `adb shell` to explore the Android file system or run commands directly.

---

## 📘 Resources
- [Android Developer ADB Guide](https://developer.android.com/studio/command-line/adb)

