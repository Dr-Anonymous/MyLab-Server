# MyLab Server (Middleware)

This repository hosts the official releases for the **MyLab Server Middleware**, the bridge between your laboratory instruments and the MyLab LIMS Cloud.

> **Note**: This is a binary distribution repository. The source code is private.

## 🚀 Installation & Setup

### 1. Download Latest Release
Go to the [Releases Page](../../releases/latest) and download the executable for your operating system:
- **Windows**: `lab-middleware-win.exe`
- **macOS**: `lab-middleware-macos`

### 2. Configuration & Linking
The Cloud URL is pre-configured. You only need to link your specific Lab Account.

1. **Run the application** (instructions below).
2. Open the Dashboard at `http://localhost:80`.
3. Click **Config** in the top right corner.
4. Enter your **Lab Master Token** (found in your LIMS Admin Panel).
5. Click **Link to Cloud**.

### 3. Running the Middleware
**Windows:**
Double-click `lab-middleware-win.exe` or run from PowerShell:
```powershell
.\lab-middleware-win.exe
```

**macOS:**
Open Terminal and run:
```bash
chmod +x lab-middleware-macos
./lab-middleware-macos
```

## 🔌 Connecting Instruments
1. Open the **Dashboard** at `http://localhost:80` (or the IP address of this machine).
2. Use the "Add Instrument" form to configure your analyzers:
   - **Name**: (e.g., "Sysmex XN-1000")
   - **Type**: (e.g., "ASTM" or "HL7")
   - **Port**: (e.g., 5001)
3. Set your Instrument's Host IP to this computer's IP and the Port you selected.

## 📋 Status & Logs
The built-in dashboard provides:
- Real-time connection status
- Live logs of data transmission
- Queue status for cloud synchronization

---
*Powered by MyLab LIMS*
