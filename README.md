# MH System Toolbox

**Professional Windows System Analysis, Optimization & Security Suite**

> A polished all-in-one toolbox for monitoring, cleaning, optimizing, and protecting Windows PCs from a single interface.

---

## Why this project stands out

MH System Toolbox brings multiple daily PC maintenance tasks into one desktop app:

- Live system dashboard with CPU, RAM, disk, and network activity
- Fast cleanup tools for temp, cache, browser, and prefetch data
- Heuristic antivirus-style scanning with process, registry, and network checks
- Driver discovery and manufacturer support links
- Startup manager, large-file finder, system reports, and optimization tools
- Optional AI assistant powered by Google Gemini
- Windows installer builds for **32-bit and 64-bit** systems

This project is designed for users who want a cleaner workflow than jumping between many separate utilities.

---

## Features

### Dashboard
- Real-time CPU, RAM, disk, and network monitoring
- Live charts and a task-manager-style overview
- Uptime, process count, and system stats at a glance

### Cleaner
- Temp file scanning and cleanup
- Cache cleanup support for common browsers
- Prefetch cleanup
- Safe deletion via Recycle Bin fallback when available

### Antivirus Engine v2
- Hash-based detection
- Heuristic file analysis
- PE/packer detection
- Entropy checks for suspicious binaries
- Suspicious script pattern scanning
- Registry autorun review
- Suspicious process detection
- Suspicious network connection checks
- Quarantine and export report support

> Note: this is a defensive scanner and triage tool, not a replacement for a full commercial endpoint security product.

### Speed Test
- Live network speed monitor
- Ookla Speedtest integration when the dependency is installed
- Upload/download testing with a clean UI

### Processes
- Process viewing and control
- CPU/RAM-focused monitoring
- Useful for troubleshooting heavy applications

### Hardware
- CPU, RAM, disk, network, battery, and system details
- Helpful for diagnostics and support

### Optimization & Gaming Mode
- Power plan switching
- RAM clearing
- DNS cache flush
- Visual effects reduction
- Temp cleanup
- Xbox Game Bar / DVR disable option
- Gaming mode profile with performance-oriented tweaks

### Drivers
- Driver inventory scan
- PC brand detection
- Direct links to manufacturer support pages
- Outdated / unsigned driver highlighting
- CSV export

### Startup Manager
- Startup items from registry Run keys and Startup folder
- Enable / disable / remove entries
- Faster startup troubleshooting

### Large File Finder
- Scan a chosen folder for space-heavy files
- Sort by size
- Delete or export results

### Reports
- Generate system reports
- Export to JSON, CSV, TXT, and HTML

### AI Assistant
- Optional Google Gemini integration
- Securely stored key using DPAPI when available
- Chat-style helper for system questions

---

## Screenshots

Add your best app screenshots here:
- Dashboard
- Cleaner
- Antivirus
- Drivers
- Optimization
- Reports

Strong screenshots will make the repository look much more mature and trustworthy.

---

## Requirements

- Windows 10 or Windows 11
- Python 3.10+ for source execution
- Administrator privileges recommended for full functionality
- Internet connection for optional features such as AI and speed testing

### Python dependencies

```bash
pip install psutil matplotlib pillow send2trash pywin32 speedtest-cli google-generativeai pystray
```

Some features are optional and will still work without their extra dependencies.

---

## Installation

### Option 1: Install from the Windows installer
Download the installer from the GitHub Releases page and run the appropriate build for your system:

- **x86 / 32-bit**
- **x64 / 64-bit**

Then launch the app from the Start Menu or desktop shortcut.

### Option 2: Run from source

```bash
git clone https://github.com/hussaini021/MH-System-Toolbox.git
cd MH-System-Toolbox
pip install -r requirements.txt
python MH_System_Suite_v1.3.py
```

---

## Usage

1. Run the application.
2. Open the page you need from the sidebar.
3. Use the action buttons to scan, clean, optimize, or export reports.
4. For advanced actions, run the app as Administrator.

---

## Project structure

```text
MH-System-Toolbox/
├── MH_System_Suite_v1.3.py   # Main application source
├── logo.png                  # App logo
├── logo.ico                  # App icon
├── installer.nsi             # Installer script
├── requirements.txt          # Python dependencies
└── README.md
```

---

## Technical notes

- Windows-only desktop application built with Tkinter
- Uses `psutil` for live system data
- Uses `matplotlib` for charts when available
- Uses `send2trash` where possible for safer deletion
- Uses DPAPI encryption for sensitive config values on Windows
- Some actions require elevation because they change system settings, registry values, or power plans

---

## Release notes

### Current build
- Modern dark UI
- Live performance dashboard
- Cleaner, driver manager, startup manager, large-file scanner
- Heuristic antivirus engine
- Optimization and gaming mode tools
- Optional Gemini AI assistant
- Installer support for both 32-bit and 64-bit Windows

---

## Limitations

- This tool is focused on Windows and is not cross-platform.
- The antivirus module is a custom heuristic scanner, not a full enterprise AV suite.
- Some optimizations can only work correctly with Administrator privileges.
- Deleting or quarantining files always carries risk; review results before confirming actions.

---

## Contributing

Contributions, fixes, and ideas are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a pull request

Please keep changes focused and tested on Windows.

---

## License

This project is released under the MIT License.

---

## Author

**Murtaza Hussaini**  
Computer Science Student · Kabul University · Information Systems Engineering

If you like the project, a star on GitHub helps a lot.
