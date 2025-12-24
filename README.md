# Passport Index Dataset (Updated Fork)

This is a fork of [ilyankou/passport-index-dataset](https://github.com/ilyankou/passport-index-dataset) with additional updates from official consular and embassy sources.

## About This Fork

This repository maintains the original passport index dataset and applies corrections based on verified embassy and consular website announcements. All updates are documented with official sources.

---

## Updates Log

### December 2025 - China Visa-Free Policy Expansion

China's unilateral visa exemption policy (30 days for ordinary passport holders):

| Passport | Change | Source |
|----------|--------|--------|
| Argentina | visa required → 30 | [National Immigration Administration](https://en.nia.gov.cn/n147418/n147463/c183390/content.html) |
| Brazil | visa required → 30 | [National Immigration Administration](https://en.nia.gov.cn/n147418/n147463/c183390/content.html) |
| Chile | visa required → 30 | [National Immigration Administration](https://en.nia.gov.cn/n147418/n147463/c183390/content.html) |
| Peru | visa required → 30 | [National Immigration Administration](https://en.nia.gov.cn/n147418/n147463/c183390/content.html) |
| Uruguay | visa required → 30 | [National Immigration Administration](https://en.nia.gov.cn/n147418/n147463/c183390/content.html) |
| Russia | visa required → 30 | [National Immigration Administration](https://en.nia.gov.cn/n147418/n147463/c183390/content.html) |

---

## Official Sources

### India (Indian passport holders)

**Source:** [Ministry of External Affairs, Government of India - Visa Facility for Indian Nationals](https://www.mea.gov.in/VFFIN.htm) | [PDF Version](https://www.mea.gov.in/images/amb1/visa-facility-for-indian-nationals.pdf)

The Ministry of External Affairs (MEA) maintains official information on visa facilities available to Indian passport holders (ordinary passports). Key highlights:

**Visa-Free Countries (23 destinations):**
- Bhutan - no limit
- Maldives - 90 days
- Nepal - no limit
- Thailand - 60 days
- Seychelles - 90 days
- Malaysia - 30 days (extended until December 31, 2026)
- Mauritius - 90 days
- Barbados - 90 days
- Dominica - 180 days
- And others

**E-Visa Countries (65 destinations):**
Including Albania, Angola, Australia, Azerbaijan, Bahrain, Cambodia, Egypt, Georgia, Hong Kong SAR, Indonesia, Japan, Jordan, Kenya (ETA as of January 2024), Mongolia, Morocco, New Zealand, Oman, Russia, Singapore, South Africa, Sri Lanka, Turkey, UAE, Vietnam, and others.

**Visa on Arrival Countries (46 destinations):**
Including Cambodia, Ethiopia, Indonesia, Jordan, Laos, Madagascar, Mauritania, Mongolia, Myanmar, Palau, Qatar, Samoa, Seychelles, Sierra Leone, Sri Lanka, Tanzania, Timor-Leste, Tuvalu, Zimbabwe, and others.

*Note: MEA recommends travelers cross-check information with the relevant Foreign Embassy/Consulate in India before travel.*

---

## Original Dataset Documentation

### About datasets

There are 6 datasets with identical visa requirements data. Three datasets are matrix and three are long (tidy) format. Each comes in 3 versions: with country codes as specified in ISO-2 (two-letter codes), ISO-3 (three-letter codes), and full country names from no particular standard.

* In distance matrices (files with `matrix` in the filename), the first column represents a passport (=from), each remaining column represents a destination (=to).
* Files in tidy format (with `tidy` in filename) have three columns: passport (from), destination (to), and the requirement.

### Dataset values

| Value | Explanation |
|---|---|
|`7`-`360`| Number of visa-free days, where available |
|`visa free`| Visa-free travel (where number of days is unknown or not applicable) |
|`visa on arrival`| Destinations that grant visa on arrival |
|`eta`| Electronic travel authorisation (ESTA, eTA, etc.) |
|`e-visa`| e-Visas (excludes ETAs) |
|`visa required`| Obtaining a visa is required for travel |
|`no admission`| Entry not permitted |
|`-1`| where passport=destination |

### Source & License

Original dataset source: https://www.passportindex.org

This fork: MIT license, same as original.
