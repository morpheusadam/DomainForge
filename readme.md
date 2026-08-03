# Domain Forge

Domain Forge is a set of Python CLI scripts that generate large lists of candidate domain names and export them as CSV files for bulk availability checking, aimed at domain investors, founders and web agencies.

## Overview

Rather than brainstorming names one at a time, the scripts produce thousands of short, dictionary-based candidates that you upload in a single batch to [Namecheap Bulk Domain Search](https://www.namecheap.com/domains/bulk-domain-search/) or any other bulk availability checker. Names are built from bundled English and Persian word lists rather than random character strings.

## Features

- Builds names from bundled English and Persian word lists.
- Generates thousands of candidates in one run.
- Splits results into multiple CSV files with a configurable batch size, to fit Namecheap upload limits.
- Uses the `Domain` header and formatting that Namecheap bulk upload expects.
- Several generation strategies: short names, super-short names, web/dev/design themed names, premium picks, and prefixed combinations.
- English and Persian (Finglish) word sources.
- No dependencies beyond the Python standard library (`csv`, `itertools`, `math`). No install or build step.

## Scripts

| Script | What it generates |
| --- | --- |
| `website.py` / `web.py` | `web + [a-z][a-z] + .com` style brandable names |
| `webdev.py` / `webdesign.py` | Developer and design themed domains |
| `short.py` / `supershort.py` | Short and ultra-short available names |
| `fadomain.py` / `7name.py` | Persian/Finglish meaningful domains (with prefix support) |
| `vip-domain.py` | Premium and high-value domain candidates |
| `check.py` / `deepcheck.py` | Availability checking helpers |

Dictionaries live in `english-words/` and `persian-words/words.txt`.

## Requirements

- Python 3.8 or higher

## Installation

```bash
git clone https://github.com/morpheusadam/DomainForge.git
cd bulk-domain-generator
```

## Usage

Run any generator script directly:

```bash
python website.py        # brandable web* domains
python short.py          # short names
python fadomain.py       # Persian/Finglish meaningful names
```

Each script writes batched CSV files (`domains_1.csv`, `domains_2.csv` and so on) into the project folder.

## Output format

CSV files follow the structure Namecheap's bulk search expects:

```csv
Domain
webaa.com
webab.com
webac.com
```

1. Open Namecheap, then Domains, then Bulk Domain Search.
2. Upload the generated `domains_*.csv`.
3. Review availability and register the names you want.

## Project structure

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

## Contributing

Open an [issue](https://github.com/morpheusadam/DomainForge/issues) or submit a pull request with new generation strategies, dictionaries, or improvements.

## License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for details.

## Author

Morpheus Adam — web developer, PHP, Laravel, Go.

- GitHub: [morpheusadam](https://github.com/morpheusadam)
- Website: [sam.zeonic.me](https://sam.zeonic.me)
- Email: morpheusadam95@gmail.com
