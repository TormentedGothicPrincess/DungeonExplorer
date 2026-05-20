# <img src="https://github.com/TormentedGothicPrincess/DungeonExplorer/blob/45208431b7582377276ae5b9eb82cd25c3ca2717/Images/about.png" width="32" height="32" alt="Launcher Icon" /> DungeonExplorer - DE is a enterprise reimagine of the Native DDO Game Launcher.

A lightweight, custom Windows 11 launcher for Dungeons & Dragons Online, leveraging data from DDO Audit to enhance the pre-game experience.

## 📸 Screenshots
<!-- 
Tip: You can drag and drop your screenshots directly into this markdown file on GitHub, and it will auto-generate the image links for you! 
-->
<img src="test" alt="Main Launcher Interface" width="300">

---

## ℹ️ About the Project
[Write a brief overview here. What problem does your launcher solve? Why did you make it? (e.g., faster loading, custom login parameters, live server population integration, etc.)]

### Key Features
* **Feature 1:** [e.g., Integrated DDO Audit live data]
* **Feature 2:** [e.g., Remembers account configurations safely]
* **Feature 3:** [e.g., Optimized for Windows 11 desktop environments]

---

## 🛠️ Technical Details & Requirements

### System Requirements
* **OS:** Windows 11 (64-bit)
* **Prerequisites:** [e.g., .NET Desktop Runtime 8.0, DirectX, etc. - leave blank if none]
* **Game:** An active installation of Dungeons & Dragons Online.

### How it Works (High-Level)
This utility acts as a wrapper around the official game executables. It fetches active server metrics from the DDO Audit API to give you real-time details before you launch the game client. 
*Note: This tool does not alter game memory, modify core game files, or bypass official patch checks.*

---

## 🚀 Download & Installation

### Step 1: Download the Release
1. Navigate to the **Releases** section on the right side of this GitHub repository.
2. Download the latest version of `[YourLauncherName].exe`.

### Step 2: Installation & First Run
1. Move the `.exe` file to your preferred directory (e.g., a dedicated folder on your Desktop or your game installation directory).
2. Launch the application. 
3. *[Optional Step]* If prompted, point the launcher to your official `TurbineLauncher.exe` or game directory.

> ⚠️ **Windows SmartScreen / Antivirus Note:** 
> Because this is a custom, unsigned binary and the source code is private, Windows Defender or your antivirus may trigger a "False Positive" warning (like SmartScreen protecting your PC). This is completely normal for independent indie tools. You may need to click *"More Info"* and *"Run Anyway"*, or add an exclusion in your antivirus settings.

---

## 🔒 Security & Verification
To ensure your download has not been tampered with, you can verify the file integrity using the SHA-256 checksum provided in the Release notes.

**How to verify via Windows PowerShell:**
```
powershell
Get-FileHash .\[YourLauncherName].exe
```

🤝 Acknowledgements & Thanks
A huge thank you to the following organizations and projects. This launcher exists because of the vibrant ecosystem and community built around the game.

Standing Stone Games & DDO
Thank you to Standing Stone Games for continuing to maintain the world of Dungeons & Dragons Online. We are incredibly grateful for their continued support of the community's freedom to create, innovate, and explore player-driven projects. It is this creative freedom that keeps the game world thriving and alive for players old and new.

DDO Audit
A massive shoutout to the team at DDOAudit for their phenomenal community resources. By providing robust, accessible APIs and data functionality, they empower independent developers to explore their own visions and build unique utilities that elevate the entire player base.
