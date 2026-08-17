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
