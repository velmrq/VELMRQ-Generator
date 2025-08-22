# VELMRQ Offline Key Generator
**Author / Project Maintainer:** Mitar Nikić
---

## Summary
This offline tool generates **2–20 secp256k1 keypairs** for your private geth-based app.  
It creates two files in the `out` folder:

1. **sendFORapp.txt** → PUBLIC data: name, address (EIP-55), pubKey (uncompressed)  
   👉 *Only this file you send to* `support@velmrq.com`  
2. **privatekey.txt** → PRIVATE data: name, address (EIP-55), pubKey, privateKey  
   👉 *Keep offline, print on paper, and delete from PC*

---

## Included Files
- `run-win.bat`, `generator_for_windows.exe`
- `run-mac.command`, `generator_for_mac`
- `run-linux.sh`, `generator_for_linux`
- `README.md` (this file)

---

## Quick Start (all OS)
1. Run the script for your OS (see below).
2. Enter a number from **2 to 20**.
3. Open the `out` folder and use the generated JSON files:
   - `sendFORapp.txt` (share with the app)
   - `privatekey.txt` (keep offline)

---

## Windows (no Python required)
- Double-click: `run-win.bat`  
- Enter 2–20  
- Open `out` → check `sendFORapp.txt` and `privatekey.txt`

---

## macOS
First time only (Terminal, in this folder):
```bash
chmod +x generator_for_mac run-mac.command
xattr -d com.apple.quarantine ./generator_for_mac   # if Gatekeeper blocks
