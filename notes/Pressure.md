# Pressure

## Definition
Atmospheric pressure is the weight of the column of air above a point, measured in hectopascals
(hPa, = millibars). MSL standard pressure is 1013.25 hPa. Pressure always decreases with
altitude, rapidly at low levels and more slowly at high altitude as air thins.

## Classification
- **QFE** — pressure setting referenced to aerodrome elevation; altimeter reads height above the
  airfield, zero on touchdown.
- **QNH** — pressure reduced to MSL using ISA conditions; altimeter reads altitude above MSL.
- **QFF** — pressure reduced to MSL using the *actual* temperature of the air column (not ISA);
  used for synoptic charts, not for altimeter setting.
- **Standard setting (1013.25 hPa)** — used above the transition altitude; altimeter reads
  **pressure altitude** / flight level.

## Formation / Key Relationships
- Pressure gradient force drives wind: closer isobars = stronger gradient = stronger wind.
- Reduction of station pressure to MSL (QNH/QFF) allows pressure comparison between stations at
  different elevations — this is what goes onto surface synoptic charts.
- Rule of thumb: pressure falls **~1 hPa per 30 ft** near MSL (~27 hPa per 1000 ft is the DGCA
  ECQB figure often quoted); the rate is *smaller* at higher levels (thinner air) than at lower
  levels — a non-linear, roughly exponential decay.
- **QNH vs QFF:** QNH always uses ISA temperature for the reduction; QFF uses actual temperature.
  If actual temperature is *below* ISA, QFF > QNH; if actual temperature is *above* ISA, QFF < QNH.

## DGCA Important Facts
- 1013.25 hPa = 29.92 in Hg = 760 mm Hg (standard atmosphere at MSL).
- An aircraft flying at a constant indicated altitude (QNH set) is actually *higher* when over
  warm air and *lower* when over cold air than the altimeter suggests, relative to true altitude
  — "high to low, look out below" applies to temperature too: **flying from warm to cold air,
  true altitude decreases below indicated.**
- Vertical spacing between pressure levels is greater in warm air, smaller in cold air (thickness
  is proportional to mean virtual temperature of the layer).

## Frequently Tested Concepts
- QNH/QFE/QFF definitions and numeric relationships in worked scenarios.
- True altitude vs pressure altitude vs density altitude vs indicated altitude — chain of
  corrections (indicated → calibration → pressure → temperature → true).
- Effect of non-standard temperature/pressure on true altitude when flying on a fixed QNH.

## Numerical Problems
- **Pressure-to-altitude, near MSL:** ~1 hPa ≈ 27–30 ft. E.g. QNH 1002 vs standard 1013.25 → 11.25
  hPa low → roughly 300 ft correction subtracted from indicated altitude to get a rough true
  picture on the day.
- **250 hPa level ≈ FL340 (~34,000 ft)** in the standard atmosphere — a commonly tested chart
  correspondence.
- **QFF from QNH:** if QNH is known and actual temperature is warmer than ISA, QFF will be
  *lower* than QNH (warm air column "weighs less" per unit reduced-to-MSL height in the QFF
  calculation) — reason through the sign, don't memorise a number.

## Memory Questions
- *For given pressure and temperature, moist air has density:* **Lower** (than dry air).
- *An increase of 1000 ft near MSL is associated with a decrease of pressure of:* **~27–33 hPa**
  (ECQB answer keys vary 27–33 depending on exact level assumed; DGCA papers have used **33 hPa**
  for the 0–1000 ft layer specifically).
- *Which would cause true altitude to increase when the altimeter indicates constant altitude?*
  **Warmer air / lower pressure region** relationship — reason from the ISA-deviation rule.

## Common Mistakes
- Mixing up QNH and QFF — QNH is what pilots set; QFF is a synoptic-chart quantity using real
  temperature.
- Assuming pressure falls linearly with height — it doesn't; the rate slows with altitude.
- Sign errors on the temperature-correction-to-true-altitude question type — always reason "ISA
  cold, true low; ISA warm, true high" from first principles rather than a memorised phrase.

## Revision Summary
Pressure falls with height, faster near the surface; QFE/QNH/QFF are three different MSL/field
references distinguished by *what* they're reduced to and *how*; temperature deviation from ISA
shifts true altitude away from indicated altitude in the same direction as the temperature
deviation.

## Supplementary (IC Joshi, ch.2 — OCR)
- **Height per 1 hPa change, by level (ISA):**

  | Level | Height per 1 hPa |
  |---|---|
  | MSL | ~27 ft |
  | 2,000 ft | ~30 ft |
  | 20,000 ft | ~50 ft |
  | 40,000 ft | ~100 ft |

  Confirms the "rate slows near the surface, widens with altitude" idea already above, now with
  concrete checkpoints — and note it's actually the *opposite* framing: the ft-per-hPa figure
  *grows* with altitude because the air is thinner (a given pressure change spans more height).
  Formula: **height per 1 hPa ≈ 96 × T(K) / p(hPa) feet.** If air is warmer than ISA, the
  height-per-hPa is larger than tabulated; if colder, smaller.
- **Static vs dynamic pressure:** static (barometric) pressure is the same in all directions in
  still air; moving air adds a directional dynamic (wind) pressure component opposing the flow —
  the distinction behind pitot-static instrument theory.
- **Semi-diurnal pressure variation** — pressure follows a bimodal daily curve: **maxima around
  1000 and 2200 local time, minima around 0400 and 1600**, lagging the temperature cycle by about
  3 hours. Amplitude is **3–5 hPa at the equator**, much smaller toward the poles. A real,
  regularly-tested "surprising fact" question (pressure minimum is *not* at the hottest time of
  day, despite lower density then, because of this ~3-hour phase lag).
