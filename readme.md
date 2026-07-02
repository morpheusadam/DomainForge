<div align="center">
# 🌐 Domain Forge
### Generate thousands of brandable, dictionary‑based domain names and export them to Namecheap‑ready CSV files — in seconds.

<p>
  <img src="https://img.shields.io/github/license/morpheusadam/DomainForge?style=for-the-badge&color=4c1" alt="License" />
  <img src="https://img.shields.io/github/stars/morpheusadam/DomainForge?style=for-the-badge&color=ffca28" alt="Stars" />
  <img src="https://img.shields.io/github/forks/morpheusadam/DomainForge?style=for-the-badge&color=42a5f5" alt="Forks" />
  <img src="https://img.shields.io/github/last-commit/morpheusadam/DomainForge?style=for-the-badge&color=8e44ad" alt="Last commit" />
  <img src="https://img.shields.io/github/repo-size/morpheusadam/DomainForge?style=for-the-badge&color=e67e22" alt="Repo size" />
</p>

<p>
  <img src="https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Output-CSV-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="CSV" />
  <img src="https://img.shields.io/badge/Namecheap-Bulk%20Search-FF6C2C?style=for-the-badge&logo=namecheap&logoColor=white" alt="Namecheap" />
  <img src="https://img.shields.io/badge/Platform-CLI-000000?style=for-the-badge&logo=gnubash&logoColor=white" alt="CLI" />
</p>

</div>

---

## 📖 Overview

**Bulk Domain Generator** is a collection of lightweight **Python CLI scripts** that generate large lists of candidate domain names and export them as **CSV files ready for [Namecheap Bulk Domain Search](https://www.namecheap.com/domains/bulk-domain-search/)** (or any bulk availability checker).

Instead of brainstorming names one by one, you can produce **thousands of meaningful, short, and brandable domains** built from real English and Persian word dictionaries, then check their availability in a single upload. It's perfect for **domain investors, indie hackers, startup founders, and web agencies** hunting for the perfect `.com`.

> 🔎 **Keywords:** bulk domain generator, domain name generator, Namecheap bulk search, available domain finder, brandable domains, domain investing, Python domain tool, CSV domain list.

---

## ✨ Features

- 🧠 **Dictionary‑driven** — builds *meaningful* names from bundled English & Persian word lists, not random gibberish.
- ⚡ **Bulk output** — generate thousands of candidates in one run.
- 🗂️ **Auto‑batching** — splits results into multiple CSV files (configurable batch size) to fit Namecheap upload limits.
- ✅ **Namecheap‑compatible** — correct `Domain` header and formatting for direct bulk upload.
- 🎯 **Multiple strategies** — short names, super‑short names, web/dev/design‑themed names, premium/VIP picks, and prefixed combinations.
- 🌍 **Bilingual** — supports both English and Persian (Finglish) word sources.
- 🪶 **Zero dependencies** — pure Python standard library (`csv`, `itertools`, `math`). No install, no build step.

---

## 🧰 Scripts

| Script | What it generates |
| --- | --- |
| `website.py` / `web.py` | `web + [a-z][a-z] + .com` style brandable names |
| `webdev.py` / `webdesign.py` | Developer & design themed domains |
| `short.py` / `supershort.py` | Short and ultra‑short available names |
| `fadomain.py` / `7name.py` | Persian/Finglish meaningful domains (with prefix support) |
| `vip-domain.py` | Premium / high‑value domain candidates |
| `check.py` / `deepcheck.py` | Availability checking helpers |

> 📁 Dictionaries live in `english-words/` and `persian-words/words.txt`.

---

## 🚀 Getting Started

### Prerequisites

- **Python 3.8+**

### Installation

```bash
git clone https://github.com/morpheusadam/DomainForge.git
cd bulk-domain-generator
```

### Usage

Run any generator script directly:

```bash
python website.py        # brandable web* domains
python short.py          # short names
python fadomain.py       # Persian/Finglish meaningful names
```

Each script writes batched CSV files (e.g. `domains_1.csv`, `domains_2.csv`, …) into the project folder.

---

## 📄 Output Format

CSV files follow the exact structure Namecheap's bulk search expects:

```csv
Domain
webaa.com
webab.com
webac.com
```

1. Open **Namecheap → Domains → Bulk Domain Search**.
2. Upload the generated `domains_*.csv`.
3. Review availability and grab your favorites. 🎉

---

## 🗂️ Project Structure

```text
bulk-domain-generator/
├── english-words/            # English dictionary source
├── persian-words/words.txt   # Persian/Finglish dictionary
├── website.py  web.py        # brandable generators
├── webdev.py  webdesign.py   # themed generators
├── short.py  supershort.py   # short-name generators
├── fadomain.py  7name.py     # Persian meaningful generators
├── vip-domain.py             # premium picks
└── check.py  deepcheck.py    # availability helpers
```

---

## 🤝 Contributing

Contributions are welcome! Open an [issue](https://github.com/morpheusadam/DomainForge/issues) or submit a pull request with new generation strategies, dictionaries, or improvements.

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

---

<div align="center">

### 👤 Author — Morpheus Adam

Web developer & cheerful hacker · PHP · Laravel · Go

<p>
  <a href="https://github.com/morpheusadam"><img src="https://img.shields.io/badge/GitHub-morpheusadam-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://sam.zeonic.me"><img src="https://img.shields.io/badge/Website-sam.zeonic.me-4c1?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="mailto:morpheusadam95@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

⭐ **If this tool helped you find your dream domain, consider giving it a star!** ⭐

</div>


---

## ⭐ Star History

<a href="https://star-history.com/#morpheusadam/DomainForge&Date">
  <img src="https://api.star-history.com/svg?repos=morpheusadam/DomainForge&type=Date" alt="bulk-domain-generator — Star History Chart" width="70%" />
</a>

<div align="center">

### If this project helps you, please give it a ⭐

A star helps other developers discover **bulk-domain-generator** and supports continued development.

</div>
