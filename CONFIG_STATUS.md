# ✅ Configuration Status Tracker

Last Updated: **2026-08-14**

## Current Config Status

| File            | Type              | Status         | Last Check | Next Check |
| --------------- | ----------------- | -------------- | ---------- | ---------- |
| `sing-box.json` | WireGuard/SingBox | ✅ **WORKING** | 2026-08-14 | 2026-08-21 |
| `warp.json`     | Hiddify/Warp      | ✅ **WORKING** | 2026-08-14 | 2026-08-21 |

---

## How to Verify Config is Working

### 🔍 Method 1: Quick Check in App (Recommended)

1. Open your VPN app (SingBox, Hiddify, etc)
2. Import the config URL
3. Click "URL Test" or "Test Connection"
4. **Green ✅ = Working** | **Red ❌ = Dead**

### 🔧 Method 2: Terminal Command

```bash
# Check if config file is accessible
curl -I https://raw.githubusercontent.com/ujanglipas/vless-try/main/sing-box.json

# Expected: HTTP/2 200 (✅ Good)
# Expected: HTTP/2 404 (❌ File not found)
```

### ⏰ Method 3: Check Expiry Date

```bash
# Look for expiry timestamp in config
# If expired, config won't work
```

---

## Import URLs

Copy these links directly to your app:

```
https://raw.githubusercontent.com/ujanglipas/vless-try/main/sing-box.json
https://raw.githubusercontent.com/ujanglipas/vless-try/main/warp.json
```

---

## Troubleshooting

**Q: Config shows ❌ Red on URL Test?**  
A: Config might be expired or server down. Check timestamp in config file.

**Q: Cannot import config?**  
A: Make sure your app supports the config protocol (WireGuard/JSON format).

**Q: Need newer config?**  
A: Pull latest from this repo or check "Next Check" date above.

---

## Auto Check Status

This file is updated automatically via GitHub Actions.  
Config files are tested every **7 days** at **00:00 UTC**.

Last auto-check: `2026-08-14 09:14:03 UTC`

---

For questions, open an issue or check the main README.md.
