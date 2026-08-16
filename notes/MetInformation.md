# Meteorological Information

## Definition
The observation, coding, and dissemination systems that deliver weather data to pilots and
controllers: routine/special reports, forecasts, charts, and broadcasts. See
`dgca_documents/METAR_TAF.md` for full code decoding.

## Classification
- **Reports (observed):** METAR (routine, hourly/half-hourly), SPECI (special, triggered by
  significant change).
- **Forecasts:** TAF (aerodrome forecast, 9/24/30 hr validity depending on use), TREND (2-hour
  landing forecast appended to a METAR/TAF), SIGMET (en-route hazardous weather: TS, severe
  turbulence/icing, volcanic ash, TRS), AIRMET (lower-severity en-route hazards below FL100/FL150).
- **Broadcasts:** VOLMET (continuous voice broadcast of METARs/TAFs for several aerodromes), ATIS
  (automated terminal information for a specific aerodrome), HF VOLMET (long-range HF version),
  ACARS (datalink).
- **Charts:** significant weather (SIGWX) charts, surface synoptic charts, upper-air charts.
- **NOTAM / SNOWTAM:** notices of hazards/field-condition changes (SNOWTAM specifically for
  runway contamination).

## Formation / Reporting Basics
- **METAR** groups (fixed order): station / time / wind / visibility / RVR / weather / clouds /
  temperature-dewpoint / QNH / trend. **CAVOK** replaces visibility, weather, and cloud groups when
  visibility ≥10 km, no cloud below 5000 ft (or the highest MSA if higher) with no CB, and no
  significant weather.
- **Temperature/dew-point group:** negative values prefixed with **M** (minus), e.g. −0.5°C/−9°C →
  **M00/M09** (each rounded to the nearest whole degree; a value that rounds to zero is expressed
  as **00**, and if actually negative it takes the M prefix even at "M00").
- **TAF validity:** commonly 9-hr (issued every 3 hr, national use) or 24/30-hr (issued every 6 hr,
  international dissemination) depending on the aerodrome category.

## DGCA Important Facts
- **CAVOK** conditions: visibility ≥10 km, no significant cloud below 5000 ft/MSA, no CB, no
  significant weather — memorise all three criteria, not just the visibility figure.
- Reading a **negative dew point that rounds to 0** still carries the **M** prefix if the actual
  value was negative (e.g. −0.5°C → M00), a classic DGCA trap question.
- **RVR** is reported in METAR (not exclusively a separate product) when visibility or RVR is at
  or below the applicable threshold.
- **TREND** covers the **2 hours** following the observation/forecast time, in TAF-like format.

## Frequently Tested Concepts
- Decoding a full METAR/TAF string, especially the temperature/dew-point group with negative
  values.
- CAVOK criteria (all three conditions, not just visibility).
- Differences between SIGMET and AIRMET (severity/altitude scope).
- VOLMET/ATIS/ACARS — what each is and how it's delivered.

## Numerical Problems
- Convert a stated air temperature/dew point pair to the correct METAR group, including sign and
  rounding rules (e.g. +0.3°C → 00; −0.3°C → M00; −0.5°C → M00 or M01 depending on rounding
  convention taught — DGCA generally rounds to nearest whole degree, half-degree ties rounding to
  the nearer even/away-from-zero convention as taught in class).

## Memory Questions
- *Dry bulb −0.5°C, dew point −9.0°C recorded at Srinagar will be reported in METAR as:*
  **M00/M09** (previously drilled as "M 00/ M 09").
- *If CAVOK is reported, then:* visibility, weather, and cloud groups are replaced — **no CB and
  no cloud below 5000 ft/MSA is implied.**
- *Validity of a TREND forecast is:* **2 hours.**

## Common Mistakes
- Forgetting the **M** prefix on a temperature/dew-point value that rounds to zero but was
  actually negative.
- Treating CAVOK as "just good visibility" and forgetting the no-CB, no-low-cloud, no-significant-
  weather requirements.
- Mixing up SIGMET (en-route hazard, all traffic) with AIRMET (lower-severity, often
  general-aviation-relevant, altitude-capped).

## Revision Summary
METAR/TAF/SPECI/TREND/SIGMET/AIRMET each serve a distinct reporting or forecasting role;
CAVOK and the negative-temperature METAR coding rules are the two most commonly mis-answered
mechanics in this topic; VOLMET/ATIS/ACARS are the delivery channels for this information to the
cockpit.

## Supplementary — Met Instruments (IC Joshi, ch.23 — OCR)
| Element | Instrument(s) | Unit |
|---|---|---|
| Pressure | Mercury barometer, aneroid barometer, barograph (self-recording) | hPa/mb (or inHg) |
| Air temperature | Dry-bulb: max (mercury) & min (alcohol) thermometer | °C |
| Dew point | Dry & wet bulb (mercury) thermometers | °C |
| Relative humidity | Dry & wet bulb thermometer, hygrometer, hygrograph, psychrometer | % |
| Humidity mixing ratio | Hygrograph | g/kg |
| Precipitation (rain) | Raingauge, self-recording raingauge, hyetograph | mm/cm |
| Precipitation (snow) | Snowgauge (by melting) | mm/cm equivalent |
| Surface wind | Wind vane (direction), anemometer (speed), anemograph (self-recording) | ° true, kt |
| Cloud base | Searchlight/laser beam, ceilometer/ceilograph, ceiling balloon | ft/m |
| Cloud movement direction | Nephoscope, alidade | 8-point compass |
| Visibility / RVR | AVRA, transmissometer, scopograph, forward scatterometer, or manual landmark method | m/km |
| Upper winds | Optical theodolite (and others for direction/speed aloft) | ° true, kt |

Useful for "which instrument measures X" question types — a distinct skill from the
transmissometer-vs-ceilometer pairing already covered above (this table is the full instrument
roster, that note is the single most commonly confused pair within it).
