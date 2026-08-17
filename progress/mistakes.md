# Mistakes Log

Claude appends an entry here after each quiz for every question answered incorrectly, and updates
existing entries if the same topic keeps recurring. Format:

```
## YYYY-MM-DD — <Topic>
**Q:** <question>
**Your answer:** <letter> — **Correct:** <letter>
**Why:** <one-line explanation>
**Seen before:** <yes/no, count>
```

## 2026-08-15 — Oktas coding
**Q:** METAR cloud cover of 6 oktas — which abbreviation?
**Your answer:** A (FEW) — **Correct:** C (BKN)
**Why:** FEW=1-2 oktas, SCT=3-4, BKN=5-7, OVC=8. 6 oktas falls in BKN range.
**Seen before:** no, count 1

## 2026-08-15 — Nacreous vs noctilucent layer
**Q:** Nacreous clouds form in which atmospheric layer?
**Your answer:** A (Mesosphere) — **Correct:** B (Upper stratosphere)
**Why:** Nacreous (mother-of-pearl) = upper stratosphere; Noctilucent = mesosphere. Classic swapped-distractor trap noted in notes/Clouds.md Common Mistakes.
**Seen before:** no, count 1

## 2026-08-15 — Nimbostratus vertical extent
**Q:** Which cloud is low-level by base but extends through medium/high levels too?
**Your answer:** D (Cirrostratus) — **Correct:** B (Nimbostratus)
**Why:** NS classified as low genus by base height but routinely extends vertically through multiple levels; CS is a pure high-level sheet cloud without this behavior.
**Seen before:** no, count 1

## 2026-08-15 — Orographic formation → lenticular cloud
**Q:** Which formation mechanism produces standing lenticular clouds over mountains?
**Your answer:** A (Convective) — **Correct:** C (Orographic/wave)
**Why:** Convective lifting produces CU→TCU→CB; forced ascent over terrain (orographic/standing-wave) produces lenticular/cap clouds.
**Seen before:** no, count 1

## 2026-08-15 — CB anvil hail hazard
**Q:** CB anvil can produce which hazard well outside the visible storm cell?
**Your answer:** A (Severe icing) — **Correct:** B (Hail)
**Why:** notes/Clouds.md DGCA Important Facts: hail under a CB anvil is a real hazard even in apparently clear air nearby.
**Seen before:** no, count 1

## 2026-08-16 — Oktas coding
**Q:** METAR sky coverage of 6 oktas — which abbreviation?
**Your answer:** B (SCT) — **Correct:** C (BKN)
**Why:** FEW=1-2 oktas, SCT=3-4, BKN=5-7, OVC=8. 6 oktas falls in the BKN range.
**Seen before:** yes, count 2 — recurring weak topic, still swapping SCT/BKN boundary.

## 2026-08-16 — Nacreous vs noctilucent layer
**Q:** Noctilucent clouds occur in which atmospheric layer?
**Your answer:** B (Stratosphere) — **Correct:** C (Mesosphere)
**Why:** Noctilucent = mesosphere (~80 km); Nacreous (mother-of-pearl) = upper stratosphere. This is the same swap trap as 2026-08-15, just asked from the other direction.
**Seen before:** yes, count 2 — persistent confusion, needs dedicated drilling.

## 2026-08-16 — Corona and Altostratus icing indication — CLEARED on 2026-08-16
**Q:** A small-radius (<5°) coloured ring around the sun/moon, duller than a halo — cause and icing implication?
**Your answer:** A (Cirrostratus — negligible icing) — **Correct:** B (Altostratus — moderate icing risk if above freezing level)
**Why:** Corona = diffraction by small water droplets/ice particles in Altostratus, indicating supercooled water → moderate icing risk. Halo (not corona) = refraction through ice crystals in Cirrostratus → negligible icing.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — CB anvil hail hazard
**Q:** Pilot flying in visually clear air under a CB anvil, away from the visible cell — hail hazard?
**Your answer:** A (Nil) — **Correct:** B (Present — hail can fall from the anvil well outside the visible cell)
**Why:** notes/Clouds.md DGCA Important Facts: hail under a CB anvil is a real hazard even in apparently clear air nearby.
**Seen before:** yes, count 2 — recurring weak topic.

## 2026-08-16 — Moist vs dry air density — CLEARED on 2026-08-16
**Q:** At the same pressure and temperature, how does moist air density compare to dry air density?
**Your answer:** C (Identical — P and T alone determine density) — **Correct:** B (Moist air is less dense)
**Why:** notes/Atmosphere.md: water vapour molecules (MW ~18) are lighter than the N₂/O₂ they displace (MW ~29), so at constant P/T moist air is less dense than dry air — density is not determined by P and T alone, composition matters too.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — ISA lapse rate numerical (sign error)
**Q:** ISA temperature at 8,000 ft (sea-level 15°C)?
**Your answer:** 1 (implied +1°C) — **Correct:** ≈ −1°C (15 − 1.98×8 = −0.84°C)
**Why:** Dropped the negative sign — at 8,000 ft under ISA the air is just below freezing, not above it. Lapse-rate arithmetic was right in method, sign discipline was the error.
**Seen before:** no, count 1

## 2026-08-16 — Stability classification (ELR vs DALR/SALR)
**Q:** ELR = 2.2°C/1000 ft, DALR ≈ 3°C/1000 ft, SALR ≈ 1.5°C/1000 ft — classify the atmosphere.
**Your answer:** A (Absolutely stable) — **Correct:** C (Conditionally unstable)
**Why:** notes/Stability.md: ELR between SALR and DALR = conditionally unstable (stable while dry, unstable once saturated). Absolutely stable requires ELR below the SALR entirely.
**Seen before:** no, count 1

## 2026-08-16 — Visibility vs synoptic pressure pattern — CLEARED on 2026-08-16
**Q:** Which synoptic pattern favours poor visibility — active Low with rain, or stagnant High/col?
**Your answer:** A (Low-pressure system with rain) — **Correct:** B (Stagnant High-pressure/col)
**Why:** notes/Visibility.md: counter-intuitively, unsettled Low-pressure weather often brings *good* visibility (rain washes out particulates, wind disperses haze); calm High-pressure/col conditions let haze/smoke/fog accumulate undisturbed — the classic DGCA reversal trap.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — CAT location relative to jet-stream core — CLEARED on 2026-08-16
**Q:** Clear Air Turbulence is most often encountered on which side of the jet core?
**Your answer:** A (Warm/equatorward side) — **Correct:** B (Cold/poleward side, near the core and tropopause)
**Why:** notes/JetStreams.md: CAT concentrates on the cold (poleward) side of the jet, near the core, near the tropopause, where shear is strongest.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Mixing ratio vs relative humidity on ascent — CLEARED on 2026-08-16
**Q:** Which quantity stays constant for an unsaturated parcel rising without gaining/losing moisture?
**Your answer:** D (Both RH and mixing ratio) — **Correct:** B (Mixing ratio only)
**Why:** notes/Thermodynamics.md: mixing ratio is conserved (no water added/removed); RH is NOT conserved — it rises as the parcel cools toward saturation. "Both" is a trap combining the two.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Mixing ratio vs absolute humidity (naming) — CLEARED on 2026-08-16
**Q:** Which quantity is mass of vapour per unit mass of dry air, unaffected by pressure/volume changes on ascent?
**Your answer:** A (Absolute humidity) — **Correct:** C (Mixing ratio)
**Why:** notes/Thermodynamics.md: absolute humidity is mass per unit *volume* (changes as the parcel expands on ascent); mixing ratio is mass per unit mass of *dry air* (conserved on ascent).
**Seen before:** no, count 1. Answered correctly on immediate retry 2026-08-16 — cleared.

## 2026-08-16 — Saturated air T/Tw/Td relationship — CLEARED on 2026-08-16
**Q:** For saturated air (fog, rain), what is the relationship between temperature, wet-bulb temperature, and dew point?
**Your answer:** A (T > Tw > Td, the unsaturated relationship) — **Correct:** B (T = Tw = Td)
**Why:** notes/Thermodynamics.md: saturated air (100% RH) has all three converge to the same value; T > Tw > Td is specifically the *unsaturated* case.
**Seen before:** no, count 1. Answered correctly on immediate retry 2026-08-16 — cleared.

## 2026-08-16 — Supercooled water droplet temperature limits — CLEARED on 2026-08-16
**Q:** Down to what temperature can supercooled water persist liquid in ordinary cloud, and in a CB?
**Your answer:** A (−10°C ordinary, −15°C in CB) — **Correct:** C (−40°C ordinary, −45°C in CB)
**Why:** notes/Thermodynamics.md / notes/Icing.md: supercooled droplets persist liquid down to about −40°C in ordinary cloud, −45°C in a CB (stronger updraughts keep droplets airborne and liquid longer).
**Seen before:** no, count 1. Answered correctly on immediate retry 2026-08-16 — cleared.

## 2026-08-16 — Primary vs secondary rainbow radius — CLEARED on 2026-08-16
**Q:** Radius of the primary rainbow (red outside, violet inside)?
**Your answer:** C (52°) — **Correct:** B (42°)
**Why:** notes/Clouds.md Optical Phenomena: primary bow = 42° radius; the fainter secondary bow (colours reversed) sits outside it at 52°. Student picked the secondary bow's radius for the primary.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Greenhouse gases — CLEARED on 2026-08-16
**Q:** Which two gases are the atmosphere's "greenhouse gases"?
**Your answer:** C (Argon and Ozone) — **Correct:** B (CO₂ and H₂O)
**Why:** notes/Atmosphere.md DGCA Important Facts: CO₂ and H₂O are the greenhouse gases — they absorb outgoing long-wave terrestrial radiation. Argon is inert; ozone's key role is stratospheric UV absorption, a separate fact.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — ISA lapse-rate cutoff altitude
**Q:** At what altitude does the ISA lapse rate (1.98°C/1000 ft) stop, becoming isothermal at −56.5°C?
**Your answer:** A (18,000 ft) — **Correct:** C (36,090 ft)
**Why:** notes/Atmosphere.md: ISA lapse rate applies up to 36,090 ft. 18,000–20,000 ft is a different fact (roughly half the atmosphere's mass lies below that level) — don't conflate the two altitude figures.
**Seen before:** no, count 1

## 2026-08-16 — Latent heat of vaporisation magnitude — CLEARED on 2026-08-16
**Q:** How much extra heat does converting boiling water to vapour need vs heating ice-cold water to boiling?
**Your answer:** D (No additional heat needed) — **Correct:** C (More than 5× as much heat)
**Why:** notes/Atmosphere.md: converting already-boiling water to vapour takes >5× the heat needed to bring the same ice-cold water to the boil — that "extra" heat is latent heat, the physical driver of cloud/storm energy release.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Ideal gas law form — CLEARED on 2026-08-16
**Q:** Which equation correctly links pressure, density, and temperature for air as an ideal gas?
**Your answer:** B (p = ρ/RT) — **Correct:** A (p = ρRT)
**Why:** notes/Atmosphere.md: pressure is directly proportional to density and temperature (p = ρRT), not inversely related.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Troposphere's share of atmospheric mass — CLEARED on 2026-08-16
**Q:** Approximately what fraction of the atmosphere's total mass is in the troposphere?
**Your answer:** D (~95%) — **Correct:** C (~75%)
**Why:** notes/Atmosphere.md: troposphere contains ~75% of atmospheric mass and nearly all weather/water vapour. Don't confuse with the separate "~half of atmospheric mass below ~18-20,000 ft" fact from notes/Fronts.md.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Mesosphere temperature trend
**Q:** How does temperature behave with height in the mesosphere?
**Your answer:** A (Increases) — **Correct:** C (Decreases)
**Why:** notes/Atmosphere.md: mesosphere temperature decreases with height again (between the warming stratosphere below and warming thermosphere above) — coldest layer overall, where noctilucent clouds form.
**Seen before:** yes, count 2 — missed again on retest 2026-08-16. Recurring weak point, needs dedicated drilling.

## 2026-08-16 — ISA lapse-rate numerical arithmetic
**Q:** ISA temperature at 12,000 ft (sea-level 15°C)?
**Your answer:** −63°C — **Correct:** ≈ −9°C (15 − 1.98×12 = −8.76°C)
**Why:** Large-magnitude arithmetic error, distinct from the earlier sign-only slip at 8,000 ft — recheck the multiplication method (1.98 × altitude-in-thousands-of-ft, not × altitude-in-ft).
**Seen before:** no, count 1 (related to a prior sign-only miss on a different altitude, but this is a distinct magnitude error)

## 2026-08-16 — Dominant atmospheric heat-transfer mechanism — CLEARED on 2026-08-16
**Q:** Which heat-transfer mechanism is dominant overall in the atmosphere?
**Your answer:** B (Convection) — **Correct:** C (Radiation)
**Why:** notes/Atmosphere.md: radiation needs no medium and drives the fundamental short-wave-in/long-wave-out energy balance — the dominant mechanism overall. Conduction matters only very near the ground; convection is important but secondary to radiation.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Fahrenheit to Celsius conversion
**Q:** Convert 86°F to Celsius.
**Your answer:** 101 — **Correct:** 30°C
**Why:** °C = (°F − 32) × 5/9 = (86−32) × 5/9 = 54 × 5/9 = 30°C. Apparent formula/arithmetic mix-up.
**Seen before:** no, count 1

## 2026-08-16 — Stefan-Boltzmann Law — CLEARED on 2026-08-16
**Q:** Radiated energy is proportional to which power of temperature?
**Your answer:** B (T²) — **Correct:** C (T⁴)
**Why:** notes/Atmosphere.md: Stefan-Boltzmann Law — radiated energy ∝ T⁴. Small temperature differences produce large radiated-energy differences (why the sun radiates so much more intensely than Earth).
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Conduction's zone of significance — CLEARED on 2026-08-16
**Q:** Where is conduction (molecular contact) significant as a heat-transfer mechanism in the atmosphere?
**Your answer:** A (Throughout the troposphere equally) — **Correct:** B (Only very near the ground)
**Why:** notes/Atmosphere.md: conduction is dominant only very near the ground; air is otherwise a poor conductor, with radiation/convection dominating away from the surface.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — ISA isothermal layer upper bound — CLEARED on 2026-08-16
**Q:** The −56.5°C isothermal layer above 36,090 ft persists up to approximately what altitude?
**Your answer:** A (45,000 ft) — **Correct:** C (65,000 ft)
**Why:** notes/Atmosphere.md: ISA lapse rate 1.98°C/1000 ft up to 36,090 ft, then constant −56.5°C up to ~65,000 ft.
**Seen before:** yes, count 2 — missed again on retest 2026-08-16 (answered 80,000 ft). Answered correctly on 3rd attempt 2026-08-16 — cleared.

## 2026-08-16 — NE Monsoon season and character — CLEARED on 2026-08-16
**Q:** The NE Monsoon affecting India blows during which season and gives what conditions?
**Your answer:** A (Summer — hot and wet) — **Correct:** B (Winter — cool and dry)
**Why:** notes/Climatology.md: NE Monsoon blows in winter, giving cool dry conditions over most of India (exception: SE coast/Tamil Nadu gets its main rains from it). Student appears to have confused it with the SW (summer) Monsoon.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Mesosphere temperature trend — CLEARED on 2026-08-16
**Q:** How does temperature behave with height in the mesosphere?
**Your answer:** A (Increases) — **Correct:** C (Decreases)
**Why:** notes/Atmosphere.md: mesosphere temperature decreases with height again — coldest layer overall.
**Seen before:** yes, count 2 — missed again on retest 2026-08-16. Answered correctly on 3rd attempt 2026-08-16 — cleared.

## 2026-08-16 — ISA lapse-rate arithmetic (persistent)
**Q:** ISA temperature at 20,000 ft (sea-level 15°C)?
**Your answer:** 11.2 — **Correct:** −24.6°C (15 − 1.98×20)
**Why:** Correct method applied successfully at 5,000 ft in the same session but broke down at 20,000 ft — check the multiplication step at larger altitude-in-thousands values; sign and magnitude both went wrong here.
**Seen before:** yes, count 3 — persistent weak point across three sessions (8,000 ft, 12,000 ft, now 20,000 ft). CLEARED on 2026-08-16 after 3 consecutive correct calculations (15,000 / 25,000 / 3,000 ft) in a dedicated drill round.

## 2026-08-16 — Argon content of dry air — CLEARED on 2026-08-16
**Q:** Approximate argon content of dry air by volume?
**Your answer:** D (~0.1%) — **Correct:** C (~1%)
**Why:** notes/Atmosphere.md: dry air is ~78% nitrogen, ~21% oxygen, ~1% argon and trace gases.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Virtual temperature: moist vs dry parcel comparison
**Q:** Same actual temperature/pressure, one dry one moist parcel — how does the moist parcel's virtual temperature compare to its actual temperature?
**Your answer:** A (Equal — virtual temp only applies to dry air) — **Correct:** B (Higher — reflects that it behaves like less-dense/warmer dry air)
**Why:** notes/Atmosphere.md: virtual temperature is the temperature dry air would need to match the density of the actual moist parcel. Moist air is less dense than dry air at the same real temperature, so the equivalent dry-air (virtual) temperature must be higher to produce that same lower density.
**Seen before:** yes, count 3 — missed again twice more on 2026-08-16 (once picking "equal" again, once picking "lower" via a density-reasoning question). Persistent misconception despite correctly explaining virtual temperature's *purpose* each time. Memory anchor given: "moist air acts warmer than it really is" → virtual temp > actual temp, always.

## 2026-08-16 — Equatorial tropopause height+temperature pairing
**Q:** How does the equatorial tropopause compare to the polar tropopause, on both height and temperature together?
**Your answer:** B (Higher and warmer) — **Correct:** C (Higher and colder)
**Why:** notes/Atmosphere.md: the two facts must be held together — the equatorial tropopause is higher AND colder simultaneously, with the greater height being the *cause* of the colder temperature (longer ascent through a falling-temperature profile), not a contradiction. Student explains the mechanism correctly when asked separately but picks the wrong combined pairing when both facts are tested together.
**Seen before:** yes, count 3 — remains unresolved despite one correct mechanism-explanation answer in the same session.

## 2026-08-16 — Equatorial tropopause paradox (height + cold, together)
**Q:** Why is the equatorial tropopause both higher AND colder than the polar tropopause?
**Your answer:** C (Only higher in summer) — **Correct:** B (Stronger convection pushes it higher; falling temperature through that longer ascent makes it colder BECAUSE it's higher)
**Why:** notes/Atmosphere.md: this is a year-round latitude effect (convective intensity), not a seasonal one. Missed twice with different wrong distractors each time.
**Seen before:** yes, count 2. Answered correctly on immediate retry 2026-08-16 (1 correct vs 2 prior misses) — improving but not yet cleared per the two-in-a-row rule; retest once more to confirm.

## 2026-08-16 — True altitude in warmer-than-ISA air — CLEARED on 2026-08-16
**Q:** Aircraft at constant indicated altitude flies into air warmer than ISA — what happens to true altitude?
**Your answer:** A (Lower than indicated) — **Correct:** B (Higher than indicated)
**Why:** notes/Pressure.md: "ISA warm, true high; ISA cold, true low." Pressure levels are more vertically spread out in warm air, so the aircraft is physically higher than the altimeter (calibrated to ISA) suggests.
**Seen before:** no, count 1. Answered correctly on immediate retry 2026-08-16 — cleared.

## 2026-08-16 — Coldest point in the vertical atmospheric profile — CLEARED on 2026-08-16
**Q:** At which layer boundary does temperature reach its overall minimum before rising again with height?
**Your answer:** A (Tropopause) — **Correct:** C (Mesopause)
**Why:** notes/Atmosphere.md: temperature falls through the troposphere, holds isothermal then rises through the stratosphere, falls again through the mesosphere to its absolute minimum at the mesopause (~85 km), then rises through the thermosphere.
**Seen before:** no, count 1. Answered correctly on immediate retry 2026-08-16 — cleared.

## 2026-08-16 — Convection vs turbulence (thermal formation mechanism) — CLEARED on 2026-08-16
**Q:** Which mechanism explains warm air rising from a sun-heated runway, forming thermals a glider can climb?
**Your answer:** D (Turbulence — eddy redistribution only) — **Correct:** B (Convection — free convection from surface heating)
**Why:** notes/Atmosphere.md: convection is organized rising current from surface heating (thermals); turbulence is chaotic eddy mixing without that organized structure.
**Seen before:** no, count 1. Answered correctly on immediate retry 2026-08-16 — cleared.

## 2026-08-16 — RH formula direction
**Q:** Which formula correctly expresses relative humidity?
**Your answer:** D (saturation vapour pressure ÷ actual vapour pressure × 100, inverted) — **Correct:** B (actual vapour pressure ÷ saturation vapour pressure × 100)
**Why:** notes/Thermodynamics.md: RH(%) = (actual HMR/vapour pressure ÷ saturated HMR/vapour pressure) × 100. Student inverted the ratio.
**Seen before:** no, count 1

## 2026-08-16 — RH formula direction — CLEARED on 2026-08-16
**Q:** Which formula correctly expresses relative humidity?
**Your answer:** D (inverted) — **Correct:** B (actual ÷ saturation vapour pressure × 100)
**Why:** notes/Thermodynamics.md: RH(%) = (actual vapour pressure ÷ saturation vapour pressure) × 100.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Dew point invariance under heating (3rd miss — applied/scenario form only)
**Q:** A parcel is heated with no moisture added/removed — what happens to its dew point?
**Your answer:** A (Rises with temperature) — **Correct:** C (Stays exactly the same)
**Why:** notes/Thermodynamics.md: dew point changes only with water-vapour content, not temperature. Warming/cooling with no moisture change alters RH but not dew point.
**Seen before:** yes, count 2. Missed a 3rd time on 2026-08-16 in concrete numeric-scenario form ("parcel cools 25°C→18°C, dew point started at 15°C — what's the dew point now?" — answered 18°C instead of 15°C), despite correctly stating the abstract rule ("dew point changes only with water-vapour content") in the very same session. CLEARED on 2026-08-16 — answered a near-identical numeric scenario (22°C→16°C, dew point 14°C) correctly in the very next session.

## 2026-08-16 — Mixing ratio vs RH on ascent (relapse)
**Q:** Which stays constant for an unsaturated rising parcel — mixing ratio or RH?
**Your answer:** C (Both remain constant) — **Correct:** B (Mixing ratio only)
**Why:** notes/Thermodynamics.md: mixing ratio is conserved; RH rises as the parcel cools toward saturation, even while unsaturated. This concept was previously cleared but relapsed with a new wrong distractor ("both").
**Seen before:** yes — previously cleared, now relapsed. Watch for "both X and Y stay constant" as a recurring trap phrasing across topics.

## 2026-08-16 — METAR negative dew point rounding (M00 vs M01)
**Q:** Dry bulb −0.5°C, dew point −9.0°C — correct METAR encoding?
**Your answer:** C (M01/M09) — **Correct:** B (M00/M09)
**Why:** notes/MetInformation.md: −0.5°C rounds to 00 in magnitude (not up to 01), but still carries the M prefix since the actual value was negative. The M prefix and the rounding are separate steps.
**Seen before:** no, count 1

## 2026-08-16 — Fog-timing calculation (formula application) — CLEARED on 2026-08-16
**Q:** Temp 30°C, dew point 20°C, cooling rate 2°C/hr — hours until fog?
**Your answer:** 10 — **Correct:** 5 hours (spread 10°C ÷ rate 2°C/hr)
**Why:** notes/Thermodynamics.md / notes/Fog.md: time to saturation = spread ÷ cooling rate. Student stated the spread (10) without completing the division.
**Seen before:** no, count 1. Answered correctly twice on retest 2026-08-16 (4 hrs and 5 hrs scenarios) — cleared.

## 2026-08-16 — Mixing ratio vs RH on ascent — RE-CLEARED on 2026-08-16
**Note:** Relapsed earlier in the session, answered correctly again on immediate retest — re-cleared.

## 2026-08-16 — METAR negative dew point rounding, small magnitude — CLEARED on 2026-08-16
**Q:** Dry bulb −0.3°C, dew point −8.0°C — correct METAR encoding?
**Your answer:** C (M01/M08) — **Correct:** B (M00/M08)
**Why:** notes/MetInformation.md: round the magnitude first, then reattach the M prefix if the original was negative. The dividing line is 0.5°C: values with magnitude <0.5 round DOWN to 00 (e.g. −0.2, −0.3, −0.4 → M00); values ≥0.5 round UP to 01 (e.g. −0.5, −0.6, −0.7 → M01).
**Seen before:** yes, count 2. Cleared on 2026-08-16 after a dedicated 4-question drill spanning both sides of the 0.5°C dividing line (−0.4→M00, −0.2→M00, −0.6→M01, −0.5→M01) — all correct once the rounding boundary was made explicit.

## 2026-08-16 — Density vs temperature at fixed pressure
**Q:** For fixed pressure, as temperature increases, air density does what?
**Your answer:** C (Unchanged) — **Correct:** B (Decreases)
**Why:** Gas law p = ρRT: at fixed p, ρ and T are inversely related — warmer air expands and becomes less dense. Directly follows from the ideal gas law form the student correctly identified earlier in the same quiz (Q1).
**Seen before:** no, count 1

## 2026-08-16 — Density altitude definition
**Q:** What is density altitude?
**Your answer:** C (Altitude where density = 1225 g/m³ everywhere) — **Correct:** B (Pressure altitude corrected for non-standard temperature)
**Why:** Density altitude = pressure altitude adjusted for temperature deviation from ISA — not a fixed density value or altitude.
**Seen before:** no, count 1

## 2026-08-16 — Horse latitudes as source of trade winds/westerlies — CLEARED on 2026-08-16
**Q:** Which feature is the source region driving both the trade winds (equatorward) and westerlies (poleward)?
**Your answer:** A (ITCZ) — **Correct:** B (Horse latitudes — subtropical high belt)
**Why:** notes/Climatology.md: horse latitudes (~30°N/S) are where descending dry air diverges, feeding trade winds toward the ITCZ and westerlies toward the polar front. ITCZ is where trade winds converge, not where either wind belt originates.
**Seen before:** no, count 1. Cleared on 2026-08-16 after a dedicated 5-question drill (divergence, ITCZ distinction, trade wind origin, westerlies origin, Hadley cell) — 5/5 correct.

## 2026-08-16 — Virtual temperature direction (persistent, 4th+ miss) — CLEARED on 2026-08-16
**Q:** Moist parcel's virtual temperature vs actual temperature, same P/T as a dry parcel?
**Your answer:** A (Equal) — **Correct:** B (Higher)
**Why:** Virtual temperature is the temperature dry air needs to match the moist parcel's density; moist air is less dense, so virtual temp is always higher. Anchor: "moist air acts warmer than it really is."
**Seen before:** yes, count 4+. Answered correctly on retest 2026-08-16 (targeted weak-topics round) — cleared after 5 total misses.

## 2026-08-16 — Equatorial tropopause height+temperature pairing (persistent, 4th+ miss) — CLEARED on 2026-08-16
**Q:** Equatorial tropopause vs polar tropopause — height and temperature together?
**Your answer:** B (Higher and warmer) — **Correct:** C (Higher and colder)
**Why:** Stronger equatorial convection drives greater height; falling temperature through that longer ascent makes it colder BECAUSE it's higher, not despite it.
**Seen before:** yes, count 4+. Answered correctly on retest 2026-08-16 (targeted weak-topics round) — cleared after 5 total misses.

## 2026-08-16 — Stability classification (persistent, now 3rd miss on the SAME scenario)
**Q:** ELR = 2.2°C/1000 ft, DALR ≈ 3°C/1000 ft, SALR ≈ 1.5°C/1000 ft — classify.
**Your answer:** A (Absolutely stable) — **Correct:** C (Conditionally unstable)
**Why:** notes/Stability.md: ELR between SALR and DALR = conditionally unstable. Student has now answered "absolutely stable" for this identical scenario on every attempt (3 total), suggesting a specific misrule: likely conflating "ELR below DALR" with "absolutely stable," when the three-way DALR/SALR comparison is what actually determines the classification (below SALR = absolutely stable; above DALR = absolutely unstable; between = conditionally unstable).
**Seen before:** yes, count 3. CLEARED on 2026-08-16 — answered correctly twice in a dedicated revision round: once with a full reasoning walkthrough, once cold on fresh numbers (ELR 2.0 vs the original 2.2°C/1000 ft scenario). Strong evidence the concept is genuinely understood now, not pattern-matched to one question.

## 2026-08-16 — Westerlies direction (from horse latitudes) — CLEARED on 2026-08-16
**Q:** Which direction do the westerlies flow?
**Your answer:** A (Horse latitudes → ITCZ) — **Correct:** B (Horse latitudes → polar front)
**Why:** notes/Climatology.md: horse latitudes feed both the trade winds (equatorward, toward ITCZ) and the westerlies (poleward, toward the polar front). Student correctly named horse latitudes as the source just 10 questions earlier in the same paper but reversed westerlies' specific direction here.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Density vs temperature at fixed pressure — CLEARED on 2026-08-16
**Note:** Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Density altitude definition — CLEARED on 2026-08-16
**Note:** Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Hail vs virga: hazard outside CB's visible boundary — CLEARED on 2026-08-16
**Q:** Which hazard can occur well outside a CB's visible boundary, including under its anvil?
**Your answer:** D (Virga) — **Correct:** C (Hail)
**Why:** notes/Precipitation.md / notes/Clouds.md: hail is exclusively a CB (convective) product and can fall from the anvil well outside the visible storm cell — a real, DGCA-tested hazard.
**Seen before:** no, count 1. Answered correctly on retest 2026-08-16 — cleared.

## 2026-08-16 — Nimbostratus as continuous-precipitation cloud — CLEARED on 2026-08-16
**Q:** Which cloud type is associated with continuous precipitation?
**Your answer:** C (Cirrus) — **Correct:** B (Nimbostratus)
**Why:** notes/Precipitation.md cloud→precipitation table: NS = continuous precipitation. Cirrus is a high-level ice-crystal cloud producing no precipitation at all.
**Seen before:** no, count 1. Answered correctly on immediate repeat-retest 2026-08-16 — cleared.

## 2026-08-16 — "Cold Day" definition (plains)
**Q:** When is a "Cold Day" declared in the plains?
**Your answer:** A (Minimum temp below 0°C) — **Correct:** B (Maximum temp ≤16°C)
**Why:** notes/Climatology.md: Cold Day = maximum temperature ≤16°C in the plains, distinct from "Cold Wave" (minimum at least 4.0°C below normal). Student conflated the two related-but-distinct winter definitions.
**Seen before:** no, count 1

## 2026-08-16 — CAVOK criteria (full three-part definition)
**Q:** What conditions must be met for CAVOK?
**Your answer:** D (Visibility ≥5000 m and no fog) — **Correct:** B (Visibility ≥10 km, no cloud below 5000 ft/MSA, no CB, no significant weather)
**Why:** notes/MetInformation.md: CAVOK requires all three criteria together — visibility, cloud, and weather — not just a visibility threshold with no fog. Classic trap where only the visibility figure is remembered.
**Seen before:** no, count 1
