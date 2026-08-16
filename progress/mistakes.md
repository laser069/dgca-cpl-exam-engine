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

## 2026-08-16 — Corona and Altostratus icing indication
**Q:** A small-radius (<5°) coloured ring around the sun/moon, duller than a halo — cause and icing implication?
**Your answer:** A (Cirrostratus — negligible icing) — **Correct:** B (Altostratus — moderate icing risk if above freezing level)
**Why:** Corona = diffraction by small water droplets/ice particles in Altostratus, indicating supercooled water → moderate icing risk. Halo (not corona) = refraction through ice crystals in Cirrostratus → negligible icing. Student conflated halo and corona.
**Seen before:** no, count 1

## 2026-08-16 — CB anvil hail hazard
**Q:** Pilot flying in visually clear air under a CB anvil, away from the visible cell — hail hazard?
**Your answer:** A (Nil) — **Correct:** B (Present — hail can fall from the anvil well outside the visible cell)
**Why:** notes/Clouds.md DGCA Important Facts: hail under a CB anvil is a real hazard even in apparently clear air nearby.
**Seen before:** yes, count 2 — recurring weak topic.

## 2026-08-16 — Moist vs dry air density
**Q:** At the same pressure and temperature, how does moist air density compare to dry air density?
**Your answer:** C (Identical — P and T alone determine density) — **Correct:** B (Moist air is less dense)
**Why:** notes/Atmosphere.md: water vapour molecules (MW ~18) are lighter than the N₂/O₂ they displace (MW ~29), so at constant P/T moist air is less dense than dry air — density is not determined by P and T alone, composition matters too.
**Seen before:** no, count 1

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

## 2026-08-16 — Visibility vs synoptic pressure pattern
**Q:** Which synoptic pattern favours poor visibility — active Low with rain, or stagnant High/col?
**Your answer:** A (Low-pressure system with rain) — **Correct:** B (Stagnant High-pressure/col)
**Why:** notes/Visibility.md: counter-intuitively, unsettled Low-pressure weather often brings *good* visibility (rain washes out particulates, wind disperses haze); calm High-pressure/col conditions let haze/smoke/fog accumulate undisturbed — the classic DGCA reversal trap.
**Seen before:** no, count 1

## 2026-08-16 — CAT location relative to jet-stream core
**Q:** Clear Air Turbulence is most often encountered on which side of the jet core?
**Your answer:** A (Warm/equatorward side) — **Correct:** B (Cold/poleward side, near the core and tropopause)
**Why:** notes/JetStreams.md: CAT concentrates on the cold (poleward) side of the jet, near the core, near the tropopause, where shear is strongest.
**Seen before:** no, count 1

## 2026-08-16 — Mixing ratio vs relative humidity on ascent
**Q:** Which quantity stays constant for an unsaturated parcel rising without gaining/losing moisture?
**Your answer:** D (Both RH and mixing ratio) — **Correct:** B (Mixing ratio only)
**Why:** notes/Thermodynamics.md: mixing ratio is conserved (no water added/removed); RH is NOT conserved — it rises as the parcel cools toward saturation. "Both" is a trap combining the two.
**Seen before:** no, count 1
