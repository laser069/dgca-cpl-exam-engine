# METAR / TAF — Decode Reference

Condensed from `Source/metar.pdf` (ICAO/WMO FM 15 format) plus DGCA syllabus points. Fixed group
order in a METAR:

```
Type  Station  Time  Wind  Visibility  RVR  Weather  Cloud  Temp/Dewpoint  QNH  Trend
```

## Example (ICAO/international format)
```
METAR LBBG 041600Z 12003MPS 290V310 1400 R04/P1500 R22/P1500U +SN BKN022 OVC050 M04/M07 Q1020 NOSIG=
```
| Group | Meaning |
|---|---|
| `METAR` | routine hourly/half-hourly report |
| `LBBG` | ICAO station identifier (Burgas, Bulgaria) |
| `041600Z` | day of month (4th), time 1600 UTC |
| `12003MPS` | wind from 120° true at 3 m/s |
| `290V310` | wind direction varying between 290° and 310° |
| `1400` | prevailing visibility 1400 m |
| `R04/P1500` | RVR runway 04: 1500 m or more, not changing significantly |
| `R22/P1500U` | RVR runway 22: 1500 m or more, and increasing (U) |
| `+SN` | heavy snow (`+`/`-` prefix = heavy/light intensity; no prefix = moderate) |
| `BKN022` | broken cloud, base 2200 ft AGL |
| `OVC050` | overcast, base 5000 ft AGL — lowest BKN/OVC layer is the reported **ceiling** |
| `M04/M07` | temperature −4°C, dew point −7°C (**M** prefix = below zero) |
| `Q1020` | QNH 1020 hPa |
| `NOSIG` | trend: no significant change expected in the next 2 hours |
| `=` | end of report |

**CAVOK** replaces the visibility/weather/cloud groups when: visibility ≥10 km, no cloud below
5000 ft or the highest minimum sector altitude (whichever is higher), no CB/TCU at any level, and
no significant weather.

## Cloud amount coding
| Code | Oktas (eighths of sky covered) |
|---|---|
| FEW | 1–2 |
| SCT | 3–4 |
| BKN | 5–7 |
| OVC | 8 |

## Temperature/dew-point group
- Two 2-digit values, whole degrees Celsius, separated by `/`.
- Negative values are prefixed with **M**, not a minus sign: −4°C → `M04`.
- A value that rounds to zero but was actually negative still takes the **M** prefix: −0.5°C →
  `M00` (a frequently tested DGCA trap — see `notes/MetInformation.md`).

## Weather intensity/qualifier prefixes
- `+` heavy, no prefix = moderate, `-` = light
- `VC` = in the vicinity (roughly 5–10 nm from the aerodrome)
- `FZ` = freezing (e.g. `FZFG` = freezing fog, `FZRA` = freezing rain)
- `SH` = showers, `TS` = thunderstorm, `BC` = patches, `DR`/`BL` = low drifting/blowing

## TAF
- Aerodrome forecast; format mirrors METAR groups but covers a validity period stated in the
  header (`e.g. 241206`, valid from the 24th 1200Z to the 25th 0600Z), with `BECMG` (gradual
  change), `TEMPO` (temporary fluctuation), `PROB30`/`PROB40` (probability) groups for expected
  variation within the period.
- Validity commonly **9 hours** (national use, issued every 3 hr) or **24/30 hours**
  (international dissemination, issued every 6 hr) depending on aerodrome category.

## TREND
- A short 2-hour forecast appended to a METAR/TAF in the same abbreviated language
  (`BECMG`/`TEMPO`/`NOSIG`), covering likely changes in the 2 hours following the observation.

## Other codes referenced in the DGCA syllabus
- **SPECI** — special report, issued when conditions cross defined significant-change thresholds
  between routine METARs (commonly cited DGCA figure: visibility crossing 3000 m, among others).
- **SIGMET** — en-route hazardous weather warning (thunderstorms, severe turbulence/icing,
  volcanic ash, tropical revolving storm) for all traffic.
- **AIRMET** — lower-severity en-route hazard warning, typically altitude-capped, aimed more at
  light/general aviation.
- **SNOWTAM** — runway surface-condition report (snow/ice/slush contamination).
- **VOLMET** — continuous voice broadcast of METAR/TAF for a list of aerodromes; **HF VOLMET** is
  the long-range HF version for oceanic/remote routes.
- **ATIS** — automated terminal information service, continuous broadcast of current aerodrome
  conditions/runway-in-use for a single aerodrome.
- **ACARS** — datalink system, among other uses, for delivering meteorological data to the cockpit.
