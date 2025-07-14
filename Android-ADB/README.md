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
## wireless debugging (Mobile side)
1. First make sure to connect with same wifi and enable wireless debugging in your phone (*android*) in developer option
   
2.Click on *pair device with pairing code*
note the ip, port and pairing code.

![WhatsApp Image 2025-07-14 at 16 59 57_2df3477d](https://github.com/user-attachments/assets/17ba7086-9ddc-435a-ba38-29fc4a2ed857)


3. Run these commands in your windows cmd *(no need for usb cable)*
```
./adb pair 192.168.x.x:port pairing-code

```
It will display device paired successfully

4.Now connect with dibugger port use the following command

![WhatsApp Image 2025-07-14 at 16 59 56_5e9b8556](https://github.com/user-attachments/assets/dd09dca1-41d5-40b7-ab75-6b4cab5f7c5d)

````
./adb connect 192.168.x.x:port
````
Your device will be connected without any error.


# 🔧 Common ADB Commands
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

