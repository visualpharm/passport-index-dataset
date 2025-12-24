# Passport Index Dataset (Updated Fork)

This is a fork of [ilyankou/passport-index-dataset](https://github.com/ilyankou/passport-index-dataset) with additional updates from official consular and embassy sources.

## About This Fork

This repository maintains the original passport index dataset and applies corrections based on verified embassy and consular website announcements. All updates are documented with official sources.

---

## Updates Log

### China

| Passport | Old | New |
|----------|-----|-----|
| Bahrain, Kuwait, Oman, Saudi Arabia, Sweden | visa required | 30 |
| Brunei | 15 | 30 |

Source: [National Immigration Administration of China](https://en.nia.gov.cn/n147418/n147463/c183390/content.html)

---

### Japan

| Passport | Old | New |
|----------|-----|-----|
| Montenegro, Paraguay, Peru | visa required | 90 |
| United Arab Emirates | 30 | 90 |

Source: [Ministry of Foreign Affairs of Japan](https://www.mofa.go.jp/j_info/visit/visa/short/novisa.html)

---

### Indonesia

| Passport | Old | New |
|----------|-----|-----|
| Brazil, Peru, Turkey | visa on arrival | 30 |

Source: [Directorate General of Immigration, Indonesia](https://www.imigrasi.go.id/berita/pemerintah-indonesia-terapkan-bebas-visa-kunjungan-bagi-warga-negara-brasil-dan-turki)

---

### Belarus

| Passport | Old | New |
|----------|-----|-----|
| Vietnam | visa required | 30 |

Source: [Embassy of Belarus in Vietnam](https://www.vietnam.mfa.gov.by/en/embassy/news/f5f4061212b78e80.html)

---

### Namibia

| Passport | Old | New |
|----------|-----|-----|
| Armenia, Australia, Austria, Azerbaijan, Belarus, Belgium, Canada, Denmark, Finland, France, Germany, Iceland, Ireland, Italy, Japan, Kazakhstan, Kyrgyzstan, Liechtenstein, Luxembourg, Moldova, Netherlands, New Zealand, Norway, Portugal, Spain, Sweden, Switzerland, Tajikistan, Turkmenistan, Ukraine, United Kingdom, United States, Uzbekistan | 90 | visa on arrival |

Source: [Embassy of Namibia in Sweden](https://embassyofnamibia.se/index.php/consular-matters/new-visa-requirements-1-april-2025)

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
