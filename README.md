# Passport Index Dataset (Updated Fork)

This is a fork of [ilyankou/passport-index-dataset](https://github.com/ilyankou/passport-index-dataset) with additional updates from official consular and embassy sources.

## About This Fork

This repository maintains the original passport index dataset and applies corrections based on verified embassy and consular website announcements. All updates are documented with official sources.

---

## Updates Log

### December 2025 - China Visa-Free Policy Expansion

China implemented unilateral visa-free entry (30 days) for the following countries:

| Passport | Change | Effective Period | Source |
|----------|--------|------------------|--------|
| Argentina | visa required → 30 | June 1, 2025 - Dec 31, 2026 | [visaforchina.cn](https://www.visaforchina.cn/DEL3_EN/tongzhigonggao/327343163872251904.html) |
| Brazil | visa required → 30 | June 1, 2025 - Dec 31, 2026 | [visaforchina.cn](https://www.visaforchina.cn/DEL3_EN/tongzhigonggao/327343163872251904.html) |
| Chile | visa required → 30 | June 1, 2025 - Dec 31, 2026 | [visaforchina.cn](https://www.visaforchina.cn/DEL3_EN/tongzhigonggao/327343163872251904.html) |
| Peru | visa required → 30 | June 1, 2025 - Dec 31, 2026 | [visaforchina.cn](https://www.visaforchina.cn/DEL3_EN/tongzhigonggao/327343163872251904.html) |
| Uruguay | visa required → 30 | June 1, 2025 - Dec 31, 2026 | [visaforchina.cn](https://www.visaforchina.cn/DEL3_EN/tongzhigonggao/327343163872251904.html) |
| Russia | visa required → 30 | Sept 15, 2025 - Sept 14, 2026 | [us.china-embassy.gov.cn](https://us.china-embassy.gov.cn/eng/lsfw/zj/notice/) |

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
