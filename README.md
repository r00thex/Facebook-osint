<h1 align="center">🕵️‍♂️ Facebook OSINT Framew</h1>

<p align="center">
  <strong>Facebook OSINT Framework</strong> to extract public profile data, business details, about information, transparency data, and more from Facebook pages using the RapidAPI Facebook Pages Scraper.
</p>

<p align="center">
  <img src="assets/MetaScan_Demo.png" title="Meta Scan Demo" alt="Meta Scan Demo" width="600"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white" alt="Python version">
  <img src="https://img.shields.io/badge/RapidAPI-API-blue?logo=rapidapi&logoColor=white" alt="RapidAPI">
  <img src="https://img.shields.io/badge/License-MIT-green?logo=open-source-initiative&logoColor=white" alt="License">
  <img src="https://img.shields.io/badge/OSINT-Facebook-blueviolet" alt="OSINT">
</p>

---

## 🚀 Features

- 🔍 **Profile Reconnaissance:** Extract full Facebook profile data (name, ID, gender, email, phone, website, followers, likes, categories, price range, description, profile/cover photos, etc.)
- 🏢 **Business Home:** Retrieve business-specific homepage details.
- 📝 **About Section:** Extract the complete "About" text of the page.
- 🔒 **Transparency Data:** Get ad status and page creation date.
- ⚡ **Fast API-Based Checking:** Powered by RapidAPI's Facebook Pages Scraper 3.
- 📄 **JSON and TXT Report Generation:** All results are saved locally with timestamps.
- 🎨 **Colored CLI Interface:** Clean and professional terminal output.
- 🔐 **Secure API Key Handling:** Credentials stored in `.env`.
- 📂 **Batch Processing:** Supports single username or batch via file (planned).
- 🕹️ **Animated Progress:** Live feedback during API calls.
- 💡 **Automatic API Setup:** Interactive onboarding via `--set-api`.
- 💰 **Donation Support:** Flag to show support links.

## 📋 Prerequisites

- Python 3.8+
- Dependencies: `requests`, `python-dotenv`, `colorama`, `urllib3`

## 🔑 API Key (RapidAPI)

Meta Scan uses the following API:

| NAME | KEY |
| ---- | --- |
| [Facebook Pages Scraper 3](https://rapidapi.com/makingdatameaningful/api/facebook-pages-scraper3) | 🔑 (Required) |

### Steps:
1. Go to [RapidAPI](https://rapidapi.com) and create a free account.
2. Subscribe to the **Facebook Pages Scraper 3** API (select the free plan).
3. Get your **API Key** from the RapidAPI dashboard.
4. Copy your API Key.

<p align="center">
  <img src="assets/MetaScan_Help.png" title="Meta Scan" alt="Meta Scan" width="600"/>
</p>

# ⚙️ Configuration

You can set your API key at any time with:

```bash
python3 fn_scan.py --set-api
```

Your key will be automatically saved in:
`.env`

<p align="center">
  <img src="assets/MetaScan_Api.png" title="Meta Scan" alt="Meta Scan" width="600"/>
</p>

---

# 💻 Usage

### 🔹 Single target (basic profile)

```bash
python3 fb_scan.py -u riatadental
```

### 🔹 Save results to JSON (creates file in ./reports)

```bash
python3 fb_scan.py -u riatadental --out-json ./reports
```

### 🔹 Donate

```bash
python3 fb_scan.py --donate
```

<p align="center">
  <img src="assets/MetaScan_Donate.png" title="Meta Scan" alt="Meta Scan" width="600"/>
</p>

---

# 📁 Reports

All results are saved in the directory specified with `--out-json`.

Example file:
`riatadental_20260820_143022_a1b2c3.json`

> [!TIP]
> **Tip:** Check the generated JSON report for advanced metadata not displayed in the terminal – for example, the full `INTRO_CARDS` object, photo lists, and all raw fields from the API.

---

# 📦 Installation

```bash
git clone https://github.com/
```
```bash
cd fb_scan
```
```bash
pip install -r requirements.txt
```

> [!WARNING]
> ## Disclaimer
> This tool is intended for **educational and OSINT research purposes only**.
> - Do not use for illegal activities.
> - The developer is not responsible for any misuse or damage caused by this tool.

---

# 📝 Notes

- The scraper extracts **publicly available data** from Facebook pages.

- The free plan of the API has usage limits – check your RapidAPI dashboard for quota.

- A **403 error** may indicate that you are not subscribed to a specific endpoint (the script now uses only endpoints available in the free plan).

- The `--no-business` flag helps avoid hitting endpoints that may require a paid subscription.

- The JSON report contains all available metadata, including fields not displayed in the terminal (e.g., full photo URLs, intro cards, etc.).

- If you encounter issues, verify your API key and subscription status.

---

> **The project is open to partners.**

# 🧪 Supported Systems
|Distribution | Verified version | 	Supported | 	Status |
|--------------|--------------------|------|-------|
|Kali Linux| 2026.2| ✅| Working   |
|ParrotOS| 7.3| ✅ | Working   |
|Windows| 11 | ✅ | Working   |
|BackBox| 9 | ✅ | Working   |
|Arch Linux| 2026.08.01 | ✅ | Working   |

## ☕️ Support the project

If you like this tool, consider buying me a coffee:

[![Buy Me a Coffee](https://img.shields.io/badge/-Buy%20me%20a%20coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/hackunderway)

---

<h2 align="center">🕵️‍♂️ OSINT Platform</h2>
<p align="center">
  <a href="https://hackunderway.io/" target="_blank">
    <img src="https://img.shields.io/badge/Try%20Enterprise%20Mode-hackunderway.io-0088CC?style=for-the-badge&logo=internet&logoColor=white" alt="OSINT Platform">
  </a>
</p>
<p align="center">
  <b>Automate OSINT processes</b><br>
  New <b>Enterprise Mode</b> – Maltego-inspired interface with visual graphs and professional workflows.<br>
  <a href="https://hackunderway.io/new-update-to-our-osint-platform-hack-underway/" target="_blank">📢 See what's new</a>
</p>
