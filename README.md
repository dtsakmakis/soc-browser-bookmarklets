# Security Browser Bookmarklets

![License](https://img.shields.io/github/license/dtsakmakis/soc-browser-bookmarklets)
![Stars](https://img.shields.io/github/stars/dtsakmakis/soc-browser-bookmarklets)
![Last Commit](https://img.shields.io/github/last-commit/dtsakmakis/soc-browser-bookmarklets)
![Repo Size](https://img.shields.io/github/repo-size/dtsakmakis/soc-browser-bookmarklets)

A collection of lightweight **browser bookmarklets** designed to speed up common workflows for:

- SOC analysts
- Threat intelligence analysts
- Incident responders
- Security researchers
- Bug bounty hunters

These tools run **directly in the browser** and require **no extensions or installation**.

---

# Live Demo

Try the bookmarklets directly in your browser:

👉 https://dtsakmakis.github.io/soc-browser-bookmarklets

From the demo page you can:

- Click bookmarklets to run them instantly
- Drag bookmarklets to your bookmarks bar
- Copy bookmarklet code manually

---

# Features

## Threat Investigation

### 🔍 IOC Search

Automatically detects the indicator type and opens relevant threat intelligence sources.

Supported indicators:

- IP addresses
- Domains
- MD5 hashes
- SHA1 hashes
- SHA256 hashes

Sources opened automatically:

- VirusTotal
- AbuseIPDB
- Whois
- Hybrid Analysis

---

### 🧠 IOC Extractor

Extract indicators directly from the current webpage.

Extracts:

- URLs
- Domains
- IP addresses
- Emails
- Hashes (MD5 / SHA1 / SHA256)

Features:

- popup interface
- filtering views
- copy to clipboard
- TXT download
- indicator counts

Useful for **triage during investigations**.

---

## Browser Utilities

### 🌐 Bulk URL Opener

Open multiple URLs in separate tabs.

Example input:

```
https://site1.com
https://site2.com
https://site3.com
```

Useful when opening:

- multiple investigation sources
- dashboards
- case references
- threat intel links

---

### 🌍 Translator

Translate selected text using **Google Translate**.

Useful when analyzing:

- foreign websites
- threat actor communications
- comments or messages
- phishing content

---

### 🔊 Speech Reader

Text-to-speech reader with a control panel.

Features:

- voice selection
- speech rate
- pitch control
- volume control
- auto language detection
- live reading highlight

Useful for accessibility or reviewing long text content.

---

### 🔢 Consecutive Numbers Generator

Generate a range of numbers and copy them to the clipboard.

Example:

```
Input:
5-10

Output:
5, 6, 7, 8, 9, 10
```

---

## Page Highlighting Tools

Highlight matching text across a page.

Available colors:

- 🟨 Yellow Highlighter
- 🟥 Red Highlighter
- 🟩 Green Highlighter

Features:

- highlight selected text
- prompt for custom text
- case-insensitive matching
- highlight across entire page

Useful when:

- reviewing large pages
- identifying keywords
- tracking indicators
- performing manual investigations

---

### 🔗 Link Highlighter

Highlights **all links on the page** for quick inspection.

Includes a floating **reset button** to remove highlights.

Useful for:

- OSINT
- page analysis
- identifying navigation paths
- spotting hidden links

---

## Highlight Cleanup Tools

Remove highlights selectively.

Available cleaners:

- Yellow Highlight Cleaner
- Red Highlight Cleaner
- Green Highlight Cleaner
- Highlight Cleaner (remove all colors)

---

# Installation

## Option 1 — Drag & Drop (Recommended)

1. Open the live demo page

https://dtsakmakis.github.io/soc-browser-bookmarklets

2. Drag any bookmarklet button to your **bookmarks bar**

3. Click the bookmarklet while browsing

---

## Option 2 — Click to Test

You can also click any bookmarklet on the demo page to run it immediately on that page.

---

## Option 3 — Copy Bookmarklet Code

If drag-and-drop is blocked:

1. Click **Copy Bookmarklet Code**
2. Create a new bookmark in your browser
3. Paste the code into the **URL / Location field**

---

# Bookmarklet Categories

The interface groups tools into categories:

| Category | Description |
|--------|--------|
| Investigation | IOC tools and threat intel helpers |
| Utilities | Browser automation and helpers |
| Highlighters | Text and link highlighting |
| Cleaners | Remove highlights |

The demo page also includes:

- 🔍 Search functionality
- 🏷 Category filtering
- 📋 Copy bookmarklet code
- 🧲 Drag-and-drop installation

---

# Example Use Cases

### SOC Investigation

Pivot an indicator into multiple threat intelligence platforms instantly.

### Threat Intelligence

Extract indicators from a webpage and analyze them quickly.

### Incident Response

Open investigation links in bulk while reviewing alerts.

### OSINT

Highlight links and keywords during research.

### Workflow Automation

Automate repetitive browser tasks without installing extensions.

---

# Designed For

- SOC Analysts
- Threat Intelligence Analysts
- Incident Responders
- Security Researchers
- Bug Bounty Hunters
- OSINT Investigators

---

# Browser Compatibility

Works with most modern browsers:

- Chrome
- Edge
- Firefox
- Brave
- Arc

Some browsers may block pop-ups the first time a bookmarklet opens multiple tabs.

If this happens, allow pop-ups for the site.

---

# Security Notice

Bookmarklets execute JavaScript in the context of the current webpage.

Always:

- review bookmarklet code
- only use bookmarklets from trusted sources

---

# License

This project is licensed under the **MIT License**.

---

⭐ If you find this project useful, consider **starring the repository**.
