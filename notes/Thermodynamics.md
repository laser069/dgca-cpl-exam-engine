# Thermodynamics (Humidity)

## Definition
The study of water vapour in the atmosphere and the heat exchanges (latent heat of
evaporation/condensation) that drive cloud, fog, and precipitation processes.

## Classification
- **Absolute humidity** — mass of water vapour per unit volume of air.
- **Mixing ratio** — mass of water vapour per unit mass of *dry* air (unaffected by
  pressure/volume changes during ascent, unlike absolute humidity — the preferred quantity for
  tracking a rising parcel).
- **Relative humidity (RH)** — ratio of actual vapour present to the maximum the air could hold at
  that temperature (saturation vapour content), expressed as %. RH = 100% at the dew point.
- **Dew point** — the temperature to which air must be cooled (at constant pressure and moisture
  content) to become saturated (RH = 100%) and begin condensing.

## Formation / Key Relationships
- Warmer air can hold more water vapour before saturating — so for a fixed actual moisture
  content, RH *falls* as temperature rises through the day and *rises* as temperature falls at
  night (this nightly RH rise, if temperature reaches the dew point, is what produces radiation
  fog/dew).
- **Temperature − dew point spread** is a direct proxy for "how close to saturation": a small
  spread means high RH and fog/cloud-formation risk; a large spread means dry air.
- Latent heat released during condensation is the energy source that slows a saturated parcel's
  cooling rate (SALR < DALR) and powers convective growth (CB).

## DGCA Important Facts
- Mixing ratio stays constant for a rising, unsaturated parcel (no water added or removed);
  relative humidity does **not** stay constant — it rises as the parcel cools toward saturation.
- The **temperature/dew-point spread narrowing toward zero** overnight, with light wind and clear
  sky, is the classic radiation-fog setup (cross-reference `notes/Fog.md`).
- Latent heat of condensation is the physical reason clouds/thunderstorms release large amounts of
  energy — the same reason SALR is less than DALR (`notes/Stability.md`).

## Frequently Tested Concepts
- Difference between mixing ratio and relative humidity, and which stays constant on ascent.
- Using the temperature/dew-point spread to judge fog/cloud risk.
- Conceptual link between latent heat release and reduced (saturated) lapse rate.

## Numerical Problems
- Given surface temperature and dew point, and an expected radiative cooling rate overnight,
  estimate the time/temperature at which saturation (fog) will occur — spread ÷ cooling rate.
- Approximate cloud base from surface spread: base (ft) ≈ 400 × (T − Td in °C) (see also
  `notes/Clouds.md`).

## Memory Questions
- *Which stays constant for an unsaturated parcel rising through the atmosphere: mixing ratio or
  relative humidity?* **Mixing ratio** (RH rises as the parcel cools).
- *Dew point is defined as:* **the temperature at which air becomes saturated (RH = 100%) at
  constant pressure and moisture content.**

## Common Mistakes
- Assuming relative humidity is conserved during ascent — it isn't; mixing ratio is.
- Treating "high humidity" (RH) and "lots of water vapour" (absolute/mixing ratio) as
  interchangeable — hot humid air and cold "humid" (near-saturated but low-absolute-moisture) air
  can have the same RH with very different actual water content.

## Revision Summary
Mixing ratio (conserved on ascent) vs relative humidity (changes with temperature) is the core
distinction; dew point marks saturation; the temperature-dew point spread is the key practical
tool for fog/cloud-base estimation; latent heat release on condensation underlies both cloud
growth and the reduced saturated lapse rate.

## Supplementary (IC Joshi, ch.5 — OCR)
- **RH formula:** RH(%) = (actual HMR ÷ saturated HMR) × 100 = (vapour pressure ÷ saturation
  vapour pressure) × 100.
- **Wet-bulb temperature (Tw)** — lowest temperature air reaches by evaporating water into it to
  saturation (desert-cooler principle: drier air → more evaporation → more cooling).
- **Dew point vs RH — the key distinguishing fact:** dew point changes **only** with water-vapour
  content; RH changes with **both** water content and temperature. So warming or cooling air with
  no moisture added/removed changes its RH but **not** its dew point.
- **State identity check** (useful for sanity-checking a METAR/synoptic reading):
  - Saturated air (fog, rain): **T = Tw = Td**
  - Unsaturated air: **T > Tw > Td**
- **Supercooled water droplet limits:** can persist liquid down to about **−40°C** in ordinary
  cloud, and down to about **−45°C** inside a CB (stronger updraughts keep droplets airborne and
  liquid longer) — the physical basis for why CB carries icing risk through such a deep layer
  (cross-reference `notes/Icing.md`).
