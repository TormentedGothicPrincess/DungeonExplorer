# <img src="https://github.com/TormentedGothicPrincess/DungeonExplorer/blob/45208431b7582377276ae5b9eb82cd25c3ca2717/Images/about.png" width="32" height="32" alt="Launcher Icon" /> DungeonExplorer 
DE is a enterprise reimagine of the Native Dungeons & Dragons Online Game Launcher.

## 📸 Screenshots
<!-- 
Tip: You can drag and drop your screenshots directly into this markdown file on GitHub, and it will auto-generate the image links for you! 
-->

<div align="center">


| Main Window | Settings |
| :---: | :---: |
|  <a href="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Main%20Window.png"><img src="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Main%20Window.png" width="350" alt="Main Window Left 1"></a>  | <a href="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Main%20Window.png"><img src="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Settings.png" width="350" alt="Main Window Left 1"></a> |

<br>


| Skin Manager | Friend Manager |
| :---: | :---: |
| <a href="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Skin%20Management.png"><img src="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Skin%20Management.png" width="350" alt="Main Window Left 1"></a> | <a href="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Friend%20Management.png"><img src="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Friend%20Management.png" width="350" alt="Main Window Left 1"></a> |

<br>

| Account Manager | Account Compendium |
| :---: | :---: |
| <a href="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Account%20Management.png"><img src="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Account%20Management.png" width="350" alt="Main Window Left 1"></a> | <a href="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Account%20Compendium.png"><img src="https://raw.githubusercontent.com/TormentedGothicPrincess/DungeonExplorer/refs/heads/main/Images/Account%20Compendium.png" width="350" alt="Main Window Left 1"></a> |

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

## 📕 The Vault: Digital Account Compendium
* The Vault (Digital Compendium): A cinematic, slide-down overlay that showcases your account's unlocked adventure packs and expansions.
* Cloud-Synced Metadata: Automatically maps raw account entitlements to rich metadata, including lore descriptions, release history, and high-resolution "book cover" art fetched from GitHub.
* Intelligent Background Caching: Features a dedicated synchronization engine that pre-fetches and caches assets locally in %AppData% using extensionless blobs for maximum performance and offline availability.
* Cinematic UI Experience: Utilizes high-performance WPF Storyboards for smooth mechanical sliding effects and elegant cross-fade transitions between library items.

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

## 💻 System Requirements:

| Component | Specification & Recommendation | Action |
| :--- | :--- | :--- |
| **Internet** | Active connection required for updates and data | [Visit ↗️](https://rog.asus.com/us/networking-group/) |
| **Operating System** | Windows 10 / 11 (Recommended: **Windows 11**) | [Download ↗️](https://www.microsoft.com/en-us/software-download/windows11) |
| **.NET Runtime** | Desktop Runtime 8.0.22+ (Recommended: **10.x**) | [Download ↗️](https://dotnet.microsoft.com/en-us/download) |
| **Base Game** | Dungeons & Dragons Online (**High Res textures** recommended) | [Visit ↗️](https://www.ddo.com/home) |
| **Native Launcher** | Required for patching and character transfers | [Download ↗️](https://www.ddo.com/guides/ddo-download) |
| **Memory (RAM)** | 8 GB of RAM (Recommended: **16 GB**) | [Visit ↗️](https://www.gskill.com/products/1/165/Desktop-Memory-U-DIMM-CU-DIMM) |
| **Graphics (GPU)** | 6 GB GPU / 100+ streams/cores (Recommended: **500+**) | [Visit ↗️](https://marketplace.nvidia.com/en-us/consumer/graphics-cards/) |
| **Storage** | 50 MB of available Hard Drive space | [Visit ↗️](https://www.samsung.com/us/memory-storage/nvme-ssd/9100-pro-nvme-ssd-sku-mz-vap2t0b-am) |
| **Audio** | Sound card or integrated audio output | [Visit ↗️](https://rog.asus.com/us/motherboards-group/) |

---

## 🚀 Download & Installation

### Step 1: Download the Release
1. Navigate to the **Releases** section on the right side of this GitHub repository.
2. Download the latest version of `DungeonExplorerInstaller.msi`.

### Step 2: Installation & First Run
1. Move the `.msi` file to your preferred directory (e.g., a dedicated folder on your Desktop or your game installation directory).
2. Launch the application. 
3. *[Optional Step]* Choose a custom install directory.

> ⚠️ **Windows SmartScreen / Antivirus Note:** 
> Because this is a custom, non-CA signed binary (self-signed) and the source code is private, Windows Defender or your antivirus may trigger a "False Positive" warning (like SmartScreen protecting your PC). This is completely normal for independent indie tools. You may need to click *"More Info"* and *"Run Anyway"*, or add an exclusion in your antivirus settings.

> ⚠️ **Limitations:** 
> 1. Patching Not Supported | <i>you will still need the Native DDO Launcher for this ). It is planned and in backlog</i>
> 2. Installation of game | <i>you will still need the Native DDO Launcher for this ). It is planned and in blacklog</i>
> 3. Character Transfers | <i>this might not be something I support, unless adoption/community feedback is positive</i>

---

## 🔒 Security & Verification
* Releases are verified by
* <img width="18" height="18" alt="image" src="https://github.com/user-attachments/assets/b83b99e4-1e52-4c42-b37d-deee99ccd869" /> Microsoft Security Intelligence
* 🛡️ VirusTotal: [0/72 Detections](https://www.virustotal.com/gui/file/your-unique-hash-here)
---
* To ensure your download has not been tampered with, you can verify the file integrity using the SHA-256 checksum provided in the Release notes as Checksum.txt

**How to verify via Windows PowerShell:**
```
powershell
Before install: -> Get-FileHash .\DungeonExplorerInstaller.msi
After install: -> Get-FileHash .\DungeonExplorer.msi.exe
```

## 🤝 Acknowledgements & Thanks

⚔️ Credits
* Producer & Lead Developer: TormentedGothicPrincess
* Music: Adventure Begins Cinematic by APALONBeats
* Font: Greyhawk Gothic by Darlene Pekul & Anna B. Meyer
* Research: ddowiki.com, ddocompendium.com, & eberron.fandom.com

❤️ Special Thanks
* Standing Stone Games & Wizards of the Coast
* The DDO Audit Team & Vault of Kundarak Team
* June Stepp (OneLauncher)
* The DDO Community Discord

</br><i>Legal Notice: This software is an unofficial, fan-made utility provided 100% free of charge. It is not affiliated with, endorsed by, or connected to Microsoft, Standing Stone Games, Wizards of the Coast, or Hasbro, Inc. All trademarks and brand names are the property of their respective owners. If you payed or were charged for this software, report it. © 2026-27 Dungeon Explorer Project. www.tormentedgothicprincess.com</i>
