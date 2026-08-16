# Atmosphere

## Definition
The atmosphere is the envelope of gases held to Earth by gravity: 78% nitrogen, 21% oxygen,
~1% argon and trace gases, plus a variable 0–4% water vapour. It is treated as an ideal gas for
aviation purposes, so pressure, temperature, and density are linked by the gas law `p = ρRT`.

## Classification
Vertical division by temperature behaviour:
- **Troposphere** — surface to the tropopause (~16–18 km at the equator, ~8–10 km at the poles,
  average ~11 km / 36,000 ft at mid-latitudes; higher in summer than winter, higher over the
  equator than the poles). Temperature falls with height (ISA lapse rate 1.98°C/1000 ft ≈
  6.5°C/km). Contains ~75% of atmospheric mass and nearly all weather and water vapour.
- **Tropopause** — boundary layer between troposphere and stratosphere; marks where the lapse
  rate changes to near-isothermal. Discontinuous (breaks) near 30° and 60° latitude, where jet
  streams form. The higher the surface temperature, the higher the tropopause.
- **Stratosphere** — tropopause to ~50 km. Temperature is isothermal in the lower part, then
  increases with height (ozone absorbing UV). Contains the ozone layer (max concentration
  20–25 km). Nacreous (mother-of-pearl) clouds occur in the upper stratosphere.
- **Mesosphere** — ~50–85 km, temperature decreases with height again. Noctilucent clouds occur
  here.
- **Thermosphere** — above ~85 km, temperature rises sharply with height (solar radiation
  absorption); very low density.

## Formation / Key Relationships
- **International Standard Atmosphere (ISA):** MSL pressure 1013.25 hPa, temperature 15°C
  (288 K), density 1225 g/m³; lapse rate 1.98°C/1000 ft (~2°C/1000 ft) up to 36,090 ft, then
  constant −56.5°C to 65,000 ft.
- **Density** depends on pressure and temperature: warmer or moister air is less dense (moist air
  is *lighter* than dry air at the same pressure/temperature — water vapour has lower molecular
  weight than dry air).
- **Additional oxygen** is required by regulation above 10,000 ft cabin altitude for extended flight.

## DGCA Important Facts
- Most atmospheric humidity and mass are concentrated in the troposphere.
- Tropopause height varies with latitude and season; it is *higher* over the equator, *lower* over
  the poles, and higher when the surface (and troposphere) is warmer.
- CO₂ and H₂O are the "greenhouse gases" of the atmosphere.
- The atmosphere is heated primarily from below (terrestrial radiation absorbed then re-radiated
  from the surface), not directly by incoming solar radiation.

## Frequently Tested Concepts
- Tropopause height vs latitude/season (equator higher & colder; poles lower & warmer at the
  tropopause itself, counter-intuitively, because the equatorial tropopause is colder in absolute
  temperature despite being higher).
- ISA temperature/pressure/density at a given level — compute or recall standard values.
- Effect of temperature/pressure on density and on true vs. pressure altitude.

## Numerical Problems
- **ISA temperature at altitude:** T = 15°C − (1.98°C × altitude in thousands of ft), valid to
  36,090 ft. E.g. at 10,000 ft: 15 − 19.8 ≈ −4.8°C ≈ −5°C.
- **Kelvin conversion:** K = °C + 273. E.g. 68°F → (68−32)×5/9 = 20°C = 293 K.

## Memory Questions
- *Lowest layer of the atmosphere is:* **Troposphere**.
- *Height of tropopause at the equator is:* **16–18 km**.
- *Minimum temperature is reached at:* **~1 hour after dawn** (not at sunrise itself — ground
  continues radiating heat away until the sun has been up a while).

## Common Mistakes
- Confusing "higher tropopause" with "warmer tropopause" — the equatorial tropopause is higher
  *and* colder than the polar tropopause.
- Forgetting the ISA lapse rate stops (goes isothermal) above 36,090 ft.
- Assuming moist air is denser than dry air — it is lighter.

## Revision Summary
Five layers by temperature behaviour (Tropo → Tropopause → Strato → Meso → Thermo); ISA is the
1013.25 hPa / 15°C / 1.98°C-per-1000ft reference; tropopause height tracks surface temperature
and latitude; density depends on pressure, temperature, and (weakly, inversely) humidity.

## Supplementary (IC Joshi, ch.3 — OCR)
- **−40°C = −40°F** — the one point the two scales agree, a handy conversion-check.
- **Virtual temperature (VT)** — the temperature a *dry* air parcel would need to match the
  pressure/density of an actual *moist* parcel; lets the dry-air gas equation be used for moist
  air too (this is the formal basis for "moist air behaves as if slightly warmer/less dense than
  dry air at the same actual temperature").
- **Heat vs temperature — not the same thing.** Heat = total kinetic energy of all molecules;
  temperature = *average* kinetic energy. A bathtub of 60°C water holds more heat than a cup of
  boiling water despite being cooler, because it has far more molecules. This is why the
  **thermosphere's very high temperatures don't heat spacecraft much** — the air is so thin
  (few, widely-spaced molecules) that its actual heat content is tiny despite the high
  temperature reading.
- **Specific heat** (heat to raise unit mass 1°C): water **1** (highest), ice **0.5**, soil **0.2**
  — this is *why* land heats and cools much faster than water/sea, the physical root of sea/land
  breeze and continental vs maritime climate behaviour (cross-reference `notes/Wind.md`,
  `notes/Climatology.md`).
- **Latent heat** — absorbed on solid→liquid→gas changes, released on the reverse. Converting
  already-boiling water to vapour takes **>5×** the heat needed to bring the same ice-cold water
  to the boil in the first place — that "extra" heat is latent and re-emerges as the physical
  driver of cloud/storm energy release (cross-reference `notes/Thunderstorms.md`,
  `notes/Stability.md`).
- **Heat transfer mechanisms in the atmosphere:** conduction (molecular contact, dominant only
  very near the ground), convection (bulk fluid transport — free convection from solar heating,
  forced convection from terrain), radiation (no medium needed — the dominant atmospheric
  mechanism overall), plus advection (horizontal, by wind), turbulence (eddy redistribution), and
  latent-heat release/absorption.
- **Radiation laws** — relevant to why the sun and earth radiate so differently:
  - **Stefan-Boltzmann Law:** radiated energy ∝ T⁴ — hot bodies (the sun) radiate far more
    intensely than cool ones.
  - **Wien's Law:** peak radiation wavelength is inversely proportional to temperature — hence the
    sun (hot) radiates mostly **short-wave** and the earth (cool) re-radiates mostly **long-wave**
    — the physical basis for "the atmosphere is heated from below" already noted above (short-wave
    solar radiation passes through relatively unimpeded; long-wave terrestrial radiation is
    absorbed by atmospheric gases).
