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
