<div align="center">
  <img src="https://raw.githubusercontent.com/novaldanorel/assets-prabowo/refs/heads/main/Screenshot%202026-09-10%20213214.png" width="300px">
</div>
<div align="center">
  <img src="https://img.shields.io/badge/Trojan-Joke-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/V1.5-green?style=for-the-badge">
  <br><br>
</div>

> **🚨 DISCLAIMER & WARNING 🚨**
> This script is a **highly disruptive prankware / joke program** created for educational purposes and controlled testing environments only. 
> 
> By running this script, it will lock system inputs, disable Task Manager, force a system restart, and spam the screen with visual glitches. **DO NOT** run this on your primary machine or any computer without the owner's explicit consent. The author is not responsible for any damage, data loss, or panic caused by the misuse of this script.

## 📝 Overview
This is a Python-based "Joke Trojan" that mimics the behavior of "screamer" or "glitch" malware. Once executed, the program persists on the system by copying itself to various directories and the Windows Startup folder. It floods the screen with unsettling glitch effects, plays disturbing audio, and prevents the user from easily closing it.

Its executable file is disguised as `crhome.exe` to make it appear like a legitimate system process.

## ✨ Features
* **Persistence & Auto-Startup:** Copies itself to `Desktop`, `Documents`, `Downloads`, and the Windows `Startup` folder.
* **First-Run Telemetry:** Sends a silent HTTP POST request to a Google Form to notify that the payload has been executed.
* **Forced Reboot:** Automatically reboots the victim's PC upon initial infection.
* **Task Manager Disable:** Continuously kills `Taskmgr.exe` and modifies the Windows Registry (`DisableTaskMgr`) to prevent the user from terminating the process.
* **Visual Glitches (Screen Spam):**
  * Rapidly changes the desktop wallpaper between red and black.
  * Spams full-screen flashing colors and "HACKED" ASCII art.
  * Captures the screen and multiplies it downwards recursively.
  * Generates an "emoji tail" that follows the mouse cursor.
* **Audio Disruption:** Plays a continuous, low-frequency (50Hz) machine hum using sine waves.
* **Input Blocking:** Blocks critical keyboard inputs (`Enter`, `Esc`, `Ctrl`, `Alt`).
* **Browser Spam:** Randomly opens chaotic websites (e.g., *youareanidiot*).

## 🛑 EMERGENCY KILL SWITCH (How to Stop It)
Since this script disables the Task Manager and blocks Ctrl and Alt, a secret kill switch has been implemented to regain control.

This will trigger the kill switch function, which re-enables the Task Manager via the Windows Registry, allowing you to manually kill the crhome.exe or Python processes.

(Note: If you would like to know about the *kill switch*, please contact me via email.)
