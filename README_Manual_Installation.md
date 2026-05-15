# Claudometer

> Know your Claude usage at a glance — right in your Chrome toolbar.

Claudometer is a free, open-source Chrome extension that shows your Claude.ai session usage as a **colour-coded icon** in your browser toolbar. Green means you're fine, amber means you're getting close, red means almost out. The number on the icon is your exact percentage.

![Claudometer icon states — green 42, amber 75, red 93](claudometer-infographic.html)

---

## What it does

- 🟢 **Green** — under 70%, keep going
- 🟡 **Amber** — 70–89%, getting close
- 🔴 **Red** — 90%+, almost out of session

Click the icon for a full breakdown showing your **5-hour session**, **weekly usage**, and **reset times** for each limit.

Updates automatically every 60 seconds. No clicking, no navigating away.

---

## Install from the Chrome Web Store

The easiest way — search **Claudometer** on the [Chrome Web Store](https://chrome.google.com/webstore) and click **Add to Chrome**.

---

## Manual installation (Developer Mode)

If you'd prefer to install directly from this repository, follow these steps. This works on **Chrome, Brave, Edge, and Arc** on both Windows and Mac.

### Step 1 — Download the files

Click the green **Code** button at the top of this page → **Download ZIP**.

Unzip the downloaded file somewhere permanent — **Documents** is ideal. Don't delete the folder after installing, Chrome needs it to stay there.

### Step 2 — Open Chrome Extensions

Type this into your Chrome address bar and press Enter:

```
chrome://extensions
```

### Step 3 — Enable Developer Mode

Toggle on **Developer Mode** using the switch in the **top-right corner** of the extensions page. A few new buttons will appear.

### Step 4 — Load the extension

Click **Load unpacked** → navigate to the folder you unzipped → select the folder that contains `manifest.json` → click **Select Folder**.

### Step 5 — Pin it to your toolbar

Click the **puzzle piece icon 🧩** in the top-right of Chrome → find **Claudometer** in the list → click the **pin 📌** next to it.

The icon will now always be visible in your toolbar.

### Step 6 — Open Claude.ai

Go to **https://claude.ai** and start or open any chat. Within 60 seconds the icon will light up with your current usage.

---

## Updating

When a new version is released, download the latest ZIP, replace your old folder with the new one, then go to `chrome://extensions` and click the **↻ reload** button on the Claudometer card.

---

## Privacy

Claudometer collects **no data whatsoever**.

- No accounts or sign-up required
- No API keys or tokens to paste
- No data sent to any third-party server
- No cookies are read — your browser handles authentication automatically
- The only things stored locally are your Claude organisation ID (cached for 24 hours) and your last usage percentages

Full privacy policy: [advaitharun101.github.io/claudometer/privacy-policy.html](https://advaitharun101.github.io/claudometer/privacy-policy.html)

---

## Permissions explained

| Permission | Why it's needed |
|---|---|
| `storage` | Saves your org ID and last-known usage locally on your device |
| `alarms` | Triggers a usage check every 60 seconds using Chrome's built-in timer |
| `claude.ai` host access | Calls Claude's internal usage API to fetch your session statistics |

---

## Built with

- Vanilla JavaScript (no frameworks, no dependencies)
- Chrome Extensions Manifest V3
- OffscreenCanvas for dynamic icon rendering

---

## License

MIT — free to use, modify, and share.
