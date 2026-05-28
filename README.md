# <img src="https://github.com/TormentedGothicPrincess/DungeonExplorer/blob/45208431b7582377276ae5b9eb82cd25c3ca2717/Images/about.png" width="32" height="32" alt="Launcher Icon" /> DungeonExplorer 
DE is a enterprise reimagine of the Native Dungeons & Dragons Online Game Launcher.

## 📸 Screenshots
<!-- 
Tip: You can drag and drop your screenshots directly into this markdown file on GitHub, and it will auto-generate the image links for you! 
-->

<div align="center">


| Top Left | Top Right |
| :---: | :---: |
| <a href="https://githubusercontent.com"><img src="https://githubusercontent.com" width="350" alt="Main Window Left 1"></a> | <a href="https://githubusercontent.com"><img src="https://githubusercontent.com" width="350" alt="Main Window Right 1"></a> |
| **Bottom Left** | **Bottom Right** |
| <a href="https://githubusercontent.com"><img src="https://githubusercontent.com" width="350" alt="Main Window Left 2"></a> | <a href="https://githubusercontent.com"><img src="https://githubusercontent.com" width="350" alt="Main Window Right 2"></a> |

</div>



---

## 🎲 Core Engine & High-Performance Launching
* Legendary Server Optimized: Tailored specifically for the newest DDO server architecture (Shadowdale, Thrane, Moonsea, Cormyr).
* Global Login System (GLS) Integration: Native C# implementation of the SOAP 1.1 authentication protocol.
* Subscription Discovery: Automatically detects and utilizes the correct Subscription ID (DDO1, etc.), bypassing character selection hang-ups.
* World Queue Gatekeeper Handshake: Performs the mandatory "Take a Number" handshake with SSG servers, solving the common "Logon Server is Full" error.
* Modern 64-Bit Support: Fully compatible with the dndclient64.exe client and modern command-line arguments.
* Smart Server Discovery: Dynamic two-step IP and Port discovery via official SSG DataCenter services.

## 👥 Advanced Account Management
* Encrypted Credential Storage: Uses Windows DPAPI (Data Protection API) to encrypt passwords specifically for the local Windows user.
* Multi-Monitor Support: Assign specific accounts to launch on specific monitors automatically (perfect for multi-boxing).
* Default Account Selection: Designate a primary account to be auto-selected upon launcher startup.
* Instant Syncing: Real-time synchronization between the Account Manager and the Dashboard selector using ObservableCollections.

## 🖥️ Session & Process Management
* PID Tracking: Automatically tracks every game instance launched through Dungeon Explorer.
* Live Performance Metrics: Monitor real-time CPU usage, Memory (Private Working Set), and Peak Memory usage per instance.
* Active Runtime Counter: Tracks exactly how long each game session has been active.
* Integrated Process Killer: Terminate specific game instances directly from the Dashboard with a single click.
* Dynamic Window Renaming: Automatically renames game windows from "Dungeons & Dragons Online" to "[AccountName]" for easy taskbar navigation.

## 📊 Live Dashboard Intelligence
* Real-Time Server Metrics: Integrated with the DDO Audit API to show live player counts and active group (LFM) counts.
* Failover Status Probing: Includes a Direct Port Probe fallback; if the API is down, the launcher pings the game servers directly to verify uptime.
* Automated Maintenance Detection: Automatically detects game-wide maintenance and blocks launch attempts to prevent client hangs.
* Live News Feed: A formatted RSS parser that pulls the latest Sales, Downtime Notices, and Release Notes directly into the UI with clickable links.

## ⚙️ Deep System Integration
* Intelligent Path Detection: Includes "Quick Find" (Registry/Steam) and "Deep Search" (recursive disk scanning) to locate game files.
* INI Configuration Management: Directly reads and writes to UserPreferences.ini to manage high-res data, 64-bit toggles, and multi-boxing permissions.
* Visual Validation: Animated status indicators provide real-time feedback during file searches and validation.
* GPU Detection: Automatically detects and lists available hardware display adapters.

## 🔒 Enterprise-Grade Security
* Digital Signature Verification: Automatically verifies that dndclient64.exe is digitally signed by Standing Stone Games before launching, preventing malware spoofing.
* NTFS Folder Lockdown: Programmatically sets ACL permissions on the AppData folder so only the authorized Windows user can access settings.
* Memory Hardening: Implements aggressive RAM clearing to ensure decrypted passwords exist in memory for only a fraction of a second.
* Anti-Debug Protection: Detects and blocks the attachment of debuggers or memory-scrapers in Release builds.

## 🎨 Modern UI/UX
* Themed WPF Interface: A completely custom-branded experience using the Greyhawk Gothic typeface.
* Borderless & Draggable: A modern, sleek window frame with custom minimize/hide-to-tray logic.
* System Tray Integration: Runs in the background with a persistent tray icon and context menu.
* Fluid Animations: GPU-accelerated XAML animations for hover effects, searching icons, and session transitions.

## Technologies Used:
* C# / .NET 8 / Windows 11
* Win32 API (User32 / Kernel32)

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

## 🤝 Acknowledgements & Thanks
A huge thank you to the following organizations and projects. This launcher exists because of the vibrant ecosystem and community built around the game.

Standing Stone Games & DDO
Thank you to Standing Stone Games for continuing to maintain the world of Dungeons & Dragons Online. We are incredibly grateful for their continued support of the community's freedom to create, innovate, and explore player-driven projects. It is this creative freedom that keeps the game world thriving and alive for players old and new.

DDO Audit
A massive shoutout to the team at DDOAudit for their phenomenal community resources. By providing robust, accessible APIs and data functionality, they empower independent developers to explore their own visions and build unique utilities that elevate the entire player base.
