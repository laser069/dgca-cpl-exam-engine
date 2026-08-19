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

## 2026-08-17 — Pressure/temperature effect on true altitude
**Q:** Flying at constant indicated altitude (QNH set) with outside air significantly colder than ISA — how does true altitude compare to indicated?
**Your answer:** C (Equal, since QNH compensates for temperature) — **Correct:** B (Lower than indicated)
**Why:** QNH reduction uses ISA temperature only, never actual temperature. Colder-than-ISA air means true altitude is below indicated ("ISA cold, true low"). Classic sign-error trap flagged in notes/Pressure.md Common Mistakes.
**Seen before:** no, count 1

## 2026-08-17 — Halo vs corona / cloud-icing mapping
**Q:** 22° radius ring around the sun, little color separation — cloud type and icing implication?
**Your answer:** D (Nimbostratus — moderate icing, continuous rain) — **Correct:** B (Cirrostratus — negligible icing, ice crystals)
**Why:** A 22° low-color ring is a halo (refraction through ice crystals in Cirrostratus), indicating negligible icing risk. Corona (not halo) is the Altostratus/moderate-icing phenomenon. notes/Clouds.md Supplementary — Optical Phenomena.
**Seen before:** no, count 1

## 2026-08-17 — CB life cycle, most hazardous stage
**Q:** Which CB life-cycle stage is most hazardous, and why?
**Your answer:** A (Cumulus stage — updraught only) — **Correct:** B (Mature stage — updraught+downdraught coexist)
**Why:** The mature stage's coexisting updraught and downdraught produce simultaneous heavy rain, hail, lightning, and severe turbulence — the peak-hazard stage. Cumulus stage has no precipitation reaching ground yet. notes/Thunderstorms.md Formation.
**Seen before:** no, count 1

## 2026-08-18 — Equatorial vs polar tropopause height/temperature
**Q:** The tropopause is higher and ___ at the equator than at the poles?
**Your answer:** A (Lower and warmer) — **Correct:** B (Higher and colder)
**Why:** Equatorial tropopause is both higher (16-18 km) and colder than the polar tropopause — "higher" does not imply "warmer." notes/Atmosphere.md Common Mistakes.
**Seen before:** no, count 1

## 2026-08-18 — Equatorial vs polar tropopause height/temperature (retest, still missed)
**Q:** Compared to the tropopause at the poles, the tropopause at the equator is (retest wording)?
**Your answer:** B (Higher and warmer) — **Correct:** C (Higher and colder)
**Why:** Same trap as above, missed again on immediate retest after revision sheet — needs a third confirmed-correct attempt before considered cleared.
**Seen before:** yes, count 2

## 2026-08-18 — RVR trend-indicator letter (U)
**Q:** In `R22/P1500U`, what does the trailing U mean?
**Your answer:** D (below 1500 m and decreasing) — **Correct:** C (1500 m or more, and increasing)
**Why:** U/D/N are RVR trend letters — increasing/decreasing/no change. The value P1500 means "1500 m or more," not below. dgca_documents/METAR_TAF.md.
**Seen before:** no, count 1

## 2026-08-18 — Wind variable-direction group
**Q:** In `08015G28KT 040V110`, what does 040V110 represent?
**Your answer:** A (wind speed varying 40-110 kt) — **Correct:** B (wind direction varying between 040° and 110°)
**Why:** A "dddVddd" group after the main wind group is always a direction-variation range, not a speed range. dgca_documents/METAR_TAF.md.
**Seen before:** no, count 1

## 2026-08-18 — TAF validity-period arithmetic
**Q:** TAF header 241206 — how should this validity period be characterized?
**Your answer:** A (9-hour national TAF) — **Correct:** B (18-hour span, 1200Z–0600Z next day, doesn't fit standard 9-hr or 24/30-hr categories)
**Why:** Day/hour arithmetic on TAF headers needs practice — this is an edge case worth recognizing rather than force-fitting to the two common categories.
**Seen before:** no, count 1

## 2026-08-18 — SIGMET vs AIRMET
**Q:** Which product is the en-route hazard warning (TS/severe turbulence/icing/volcanic ash/TRS) for all traffic?
**Your answer:** A (AIRMET) — **Correct:** B (SIGMET)
**Why:** SIGMET = severe hazards, all traffic. AIRMET = lower-severity, altitude-capped, more GA-relevant. dgca_documents/METAR_TAF.md.
**Seen before:** no, count 1

## 2026-08-18 — SNOWTAM purpose
**Q:** What does SNOWTAM report?
**Your answer:** A (upper-level wind forecasts) — **Correct:** B (runway surface contamination — snow/ice/slush)
**Why:** SNOWTAM is specifically a runway-condition report, unrelated to wind forecasts. dgca_documents/METAR_TAF.md.
**Seen before:** no, count 1

## 2026-08-18 — SIGMET vs AIRMET (retest, still missed)
**Q:** Moderate turbulence below FL100, mainly for GA traffic, lower severity than a full en-route hazard warning — which product?
**Your answer:** A (SIGMET) — **Correct:** B (AIRMET)
**Why:** Same trap as the first attempt — AIRMET is specifically the lower-severity, altitude-capped, GA-relevant product; SIGMET is for severe hazards affecting all traffic. This is now the clearest single recurring gap in METAR/TAF.
**Seen before:** yes, count 2

## 2026-08-18 — ACARS vs VOLMET distinction
**Q:** Which delivery system is a datalink service delivering met data to the cockpit without voice communication?
**Your answer:** B (VOLMET) — **Correct:** C (ACARS)
**Why:** ACARS is the datalink system; VOLMET is the continuous *voice* broadcast of METARs/TAFs. Both deliver weather data to aircraft, but the mechanism (datalink vs voice) is the distinguishing fact. dgca_documents/METAR_TAF.md.
**Seen before:** no, count 1

## 2026-08-18 — BC (patches) qualifier
**Q:** What does the BC qualifier mean in a group like BCFG?
**Your answer:** C (Before — occurred just prior to observation) — **Correct:** B (Patches — irregular, patchy coverage of the phenomenon)
**Why:** BC is a coverage/distribution qualifier (patches), not a timing indicator. dgca_documents/METAR_TAF.md.
**Seen before:** no, count 1

## 2026-08-18 — Layer thickness, warm vs cold air
**Q:** Vertical spacing (thickness) between two pressure levels is greater in which air mass?
**Your answer:** A (Cold air) — **Correct:** B (Warm air)
**Why:** Warm air is less dense, so a given pressure change spans more height — thickness is greater in warm air. notes/Pressure.md / notes/Fronts.md.
**Seen before:** no, count 1

## 2026-08-18 — Friction effect on surface wind
**Q:** Compared to gradient wind aloft, surface wind due to friction (NH)?
**Your answer:** A (Backs and increases in speed) — **Correct:** C (Backs and decreases in speed)
**Why:** Friction backs AND slows surface wind relative to the gradient wind aloft — speed decreases, not increases. notes/Wind.md.
**Seen before:** no, count 1

## 2026-08-18 — Nimbostratus multi-level classification (recurrence)
**Q:** Which cloud genus is classified low-level by base but extends through medium/high levels?
**Your answer:** D (Stratocumulus) — **Correct:** B (Nimbostratus)
**Why:** Same trap as 2026-08-15 entry — Nimbostratus, not Stratocumulus, extends vertically through multiple levels despite a low base classification.
**Seen before:** yes, count 2

## 2026-08-18 — Inversion effect on vertical mixing
**Q:** A temperature inversion is associated with?
**Your answer:** A (Strong convective cloud development) — **Correct:** B (Suppressed vertical mixing, trapping fog/haze below)
**Why:** Inversions are extremely stable and suppress vertical mixing — they trap pollutants/fog beneath them rather than encouraging convection. notes/Stability.md.
**Seen before:** no, count 1

## 2026-08-18 — Cold occlusion air-mass temperature logic
**Q:** In a cold occlusion, which air mass is colder — behind or ahead of the front?
**Your answer:** B (Air behind is warmer, warm-front characteristics dominate) — **Correct:** A (Air behind is colder, cold-front characteristics dominate)
**Why:** By definition, a *cold* occlusion has colder air behind the front than ahead of it, so cold-front weather dominates at the surface. notes/Fronts.md.
**Seen before:** no, count 1

## 2026-08-18 — India's dominant winter air mass
**Q:** Which air mass, originating from the Siberian high, dominates over India in winter (cold, dry, hazy)?
**Your answer:** B (Tropical Maritime, Tm) — **Correct:** C (Tropical Continental, Tc)
**Why:** Tc (Tropical Continental) is India's dominant winter air mass, sourced from the Siberian high. Tm (Tropical Maritime) is the moist, SE-Asia-sourced monsoon-season air mass instead. notes/Fronts.md Supplementary.
**Seen before:** no, count 1

## 2026-08-18 — TRS energy source
**Q:** The primary energy source for a Tropical Revolving Storm is?
**Your answer:** A (Direct solar heating of cloud tops) — **Correct:** B (Latent heat release from condensation over warm ocean water)
**Why:** TRS draws energy from latent heat released as moist air condenses over warm (>26-27°C) ocean water, not from direct solar heating. notes/PressureSystems.md.
**Seen before:** no, count 1
