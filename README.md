# Security Browser Bookmarklets

Collection of lightweight browser bookmarklets designed to speed up common workflows for **security analysts, SOC operations, and everyday browsing automation**.

These bookmarklets run directly in the browser and **require no extensions or installations**.

---

## Features

* 🔍 **IOC quick search** (VirusTotal / AbuseIPDB / Whois / Hybrid Analysis)
* 🌐 **Bulk URL opener**
* 🌎 **Text translator**
* 🔢 **Consecutive numbers generator**
* 🟨🟥🟩 **Text highlighters** (yellow / red / green)
* 🧹 **Highlight cleaner**
* 🔊 **Speech reader**

---

## Installation

1. Copy the JavaScript code from the bookmarklet file.
2. Create a new bookmark in your browser.
3. Paste the JavaScript code into the **URL / Location** field.
4. Click the bookmarklet while browsing to execute it.

Works with most modern browsers:

* Chrome
* Edge
* Firefox
* Brave

---

## Example Use Cases

* SOC investigations
* Threat intelligence lookups
* Quick IOC enrichment
* Browser task automation
* Page content highlighting

---

## IOC Search Bookmarklet

This bookmarklet automatically detects the type of **Indicator of Compromise (IOC)** and opens relevant threat intelligence sources.

### Supported IOC Types

* IP addresses
* Domains
* MD5 hashes
* SHA1 hashes
* SHA256 hashes

### Intelligence Sources Opened

* VirusTotal
* AbuseIPDB
* Hybrid Analysis
* Whois

---

## Bookmarklets

Drag the links below to your bookmarks bar.

- [IOC Search](javascript:!function(){try{const e=(getSelection?getSelection().toString():"").trim(),t=(e||prompt("IOC?")||"").trim();if(!t)return;const o=encodeURIComponent(t),n=/^(?:25[0-5]|2[0-4]\d|1?\d?\d)(?:\.(?:25[0-5]|2[0-4]\d|1?\d?\d)){3}$/.test(t),r=/^(?:[A-Fa-f0-9]{1,4}:){2,7}[A-Fa-f0-9]{1,4}$/.test(t),a=/^(?:https?|ftp):\/\//i.test(t),c=/^[A-Fa-f0-9]{64}$/.test(t),i=/^[A-Fa-f0-9]{40}$/.test(t),s=/^[A-Fa-f0-9]{32}$/.test(t),f=c||i||s,d=!a&&/^[A-Za-z0-9-]{1,63}(\.[A-Za-z0-9-]{1,63})+\.?$/.test(t);let l=[];if(n||r)l=[`https://www.virustotal.com/gui/search/${o}`,`https://www.abuseipdb.com/check/${o}`];else if(d){const e=t.replace(/\.$/,"");l=[`https://www.virustotal.com/gui/search/${encodeURIComponent(e)}`,`https://www.whois.com/whois/${e}`]}else{if(!f)return void alert("Unsupported input. Enter IP, domain, or MD5/SHA1/SHA256 hash.");l=[`https://www.virustotal.com/gui/search/${o}`,`https://www.hybrid-analysis.com/search?query=${o}`]}[...new Set(l)].forEach(e=>window.open(e,"_blank"))}catch(e){alert("IOC launcher error: "+e)}}();)
- [Bulk URL Opener](javascript:(()=>{const txt=prompt('Paste URLs (one per line)');if(!txt)return;const urls=txt.split(/\s+/).filter(Boolean);for(const u of urls){const href=/^https?:\/\//i.test(u)?u:%27https://%27+u;window.open(href,%27_blank%27)}})();)
- [Translator](javascript:(function() {  let text = window.getSelection().toString();  if (!text) return alert("Please select some text first.");  window.open("https://translate.google.com/?sl=auto&tl=en&text=" + encodeURIComponent(text));})();)
- [Speech Reader](javascript:(function(){  let text = window.getSelection().toString();  if (!text) return alert("Select some text first.");  let msg = new SpeechSynthesisUtterance(text);  speechSynthesis.speak(msg);})();)

---

## Disclaimer

Bookmarklets execute JavaScript in the context of the current webpage.
Only use bookmarklets from **trusted sources**.

---

## License

This project is licensed under the MIT License.
