# Formulas & Quick Reference — Aviation Meteorology

## International Standard Atmosphere (ISA)
- MSL: pressure **1013.25 hPa**, temperature **15°C (288 K)**, density **1225 g/m³**
- Lapse rate (surface → 36,090 ft): **1.98°C / 1000 ft ≈ 2°C / 1000 ft** (≈6.5°C/km)
- Above 36,090 ft to 65,000 ft: isothermal at **−56.5°C**
- `T(°C) at altitude ≈ 15 − 1.98 × (altitude in thousands of ft)`  — valid below 36,090 ft

## Temperature Conversion
- `°F → °C: (°F − 32) × 5/9`
- `°C → °F: (°C × 9/5) + 32`
- `°C → K: °C + 273 (273.15 precise)`

## Pressure / Altitude
- 1013.25 hPa = 29.92 inHg = 760 mmHg
- Near MSL: **~1 hPa ≈ 27–30 ft**; DGCA ECQB often uses **33 hPa per 1000 ft** for the 0–1000 ft
  layer specifically — the rate *decreases* with altitude (non-linear).
- 250 hPa level ≈ **FL340** in the standard atmosphere (commonly tested chart correspondence).
- **QNH** = pressure reduced to MSL using ISA temperature.
- **QFF** = pressure reduced to MSL using actual (real) temperature.
  - Actual temp < ISA → QFF > QNH
  - Actual temp > ISA → QFF < QNH
- **QFE** = pressure at aerodrome elevation (altimeter reads 0 on the runway).
- Altitude correction rule: flying at fixed indicated altitude (QNH set), true altitude moves in
  the *same direction* as the temperature deviation from ISA (warmer than ISA → true altitude
  higher than indicated; colder than ISA → true altitude lower than indicated — "cold air, look
  out below below the level you think you're at").

## Stability / Lapse Rates
- **DALR (Dry Adiabatic Lapse Rate):** ≈ **3°C / 1000 ft** (9.8°C/km)
- **SALR (Saturated Adiabatic Lapse Rate):** ≈ **1.5°C / 1000 ft** (~5°C/km, varies with
  temperature/moisture — smaller than DALR because condensation releases latent heat)
- **ELR (Environmental Lapse Rate)** — the actual observed rate on the day; compare to DALR/SALR:
  - ELR < SALR → absolutely stable
  - ELR > DALR → absolutely unstable
  - SALR < ELR < DALR → conditionally unstable

## Humidity / Cloud Base
- **Cloud base (approx., convective condensation level):** `base (ft) ≈ 400 × (T − Td, in °C)`
  where T = surface temperature, Td = surface dew point
- **Mixing ratio** — conserved for an unsaturated rising parcel; **relative humidity** is not
  (RH rises as the parcel cools toward saturation).

## METAR Coding
- Cloud amount: **FEW** 1–2 oktas · **SCT** 3–4 oktas · **BKN** 5–7 oktas · **OVC** 8 oktas
- Negative temperature/dew point: prefix **M** (e.g. −0.5°C ≈ **M00** rounded, −9°C = **M09**)
- **CAVOK**: visibility ≥10 km, no cloud below 5000 ft/MSA (whichever higher), no CB, no
  significant weather
- **TREND**: forecast covering the **2 hours** following the report/forecast time

## Wind
- Coriolis force: **zero at the equator, maximum at the poles**, proportional to wind speed
- Surface wind (vs. gradient wind aloft): backs (NH) and slows due to friction, blows slightly
  across isobars toward low pressure
- **Buys Ballot's Law (NH):** back to the wind → low pressure is on your left

## Icing
- Most favourable icing temperature band: **0°C to −20°C**
- Heaviest icing risk: **Cumulonimbus (CB)**

## Miscellaneous DGCA-Favourite Numbers
- Additional oxygen required above **10,000 ft** cabin altitude
- Roughly half the atmosphere's mass lies below **~18,000–20,000 ft**
- Gale: sustained wind **> 33 kt**, associated with a depression
- Fog: visibility **< 1000 m**; Mist: **1000–5000 m** with RH near 100%
- SPECI trigger (DGCA ECQB figure): visibility crossing **3000 m**
