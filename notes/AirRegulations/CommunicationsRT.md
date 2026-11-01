# CommunicationsRT

Study notes built only from the source text in `D:/Quiz App/build/raw_text/`. Source tags are file names without extension. Pool answers are shown only when the pool Confidence line is verified/matched/derived, and each is labelled. CommunicationsRT pool: 0 verified, 0 matched, 35 derived (model-worked, NOT an official key), 5 unresolved.

## Definition

- **Two-way communication (controlled flight)**: "A controlled flight is required to maintain two way RTF communications with the controlling ATCU." (src: zenithaviation_regsnotes, notes_air_regs_nirmal_firosh)
- **Watch requirement**: a controlled aircraft "shall maintain continuous air-ground voice communication watch on the appropriate communication channel and establish two-way communication as necessary." SELCAL or similar automatic signalling satisfies the watch requirement. (src: notes_air_regs_vinod_yadav)
- **Radar contact**: "the aircraft has been identified on the radar display and radar flight instructions will be provided until termination." (src: zenithaviation_regsnotes)
- **Resume own navigation**: "use your Navigation facility for Navigation." (src: zenithaviation_regsnotes)
- **ATIS (Automatic Terminal Information Service)**: "a voice broadcast of current weather of the aerodrome within 5 NM radius and 5000 ft (1500 m) height." (src: zenithaviation_regsnotes)
- **Aircraft call sign**: "in radiotelephony the call sign to be used by the aircraft will consist of this identification alone" or the flight identification number (src: notes_air_regs_vinod_yadav).

## Classification

- **Communication channels**: VHF voice (air-ground), UHF, and emergency/guard frequencies 121.5 MHz and 243.0 MHz (src: notes_air_regs_vinod_yadav, notes_air_regs_nirmal_firosh).
- **SSR transponder modes**: Mode A (4 digits, 4096 codes) and Mode C (Mode A plus pressure altitude) (src: notes_air_regs_vinod_yadav, zenithaviation_regsnotes).
- **Special-purpose SSR codes**: 7700 (emergency/distress), 7600 (radio failure), 7500 (hijack / unlawful interference) (src: notes_air_regs_vinod_yadav, zenithaviation_regsnotes).
- **Aircraft weight categories for R/T call signs**: Heavy, Medium, Light (src: zenithaviation_regsnotes).
- **Light signals from control tower**: steady and flashing red/green/white for aircraft in flight and on ground (src: zenithaviation_regsnotes).

## Formation

How the R/T and SSR procedures are built (background from the sources):

- A controlled flight keeps a continuous watch on the ATC frequency; in a communication failure the aircraft uses the transponder code and the last assigned speed/level to tell ATC what is happening (src: notes_air_regs_vinod_yadav, zenithaviation_regsnotes).
- The transponder is the main link for radar: Mode A gives the code; Mode C adds pressure altitude; IDENT is used only when ATC asks (src: zenithaviation_regsnotes).
- Radio failure is handled in two cases: VMC (fly on, land at nearest suitable aerodrome) and IMC (squawk 7600, hold last speed and level, proceed on flight plan, land within 30 min of ETA) (src: notes_air_regs_vinod_yadav, notes_air_regs_nirmal_firosh).
- Intercept signals are visual/radio: the intercepting aircraft uses 121.5 MHz; the intercepted aircraft squawks 7700 unless ATS instructs otherwise (src: air_regulations_4).

## DGCA Important Facts

- Transponder must be operated at all times during flight, whether or not inside SSR-used airspace (src: air_regulations_4).
- Within the Chennai, Delhi, Guwahati, Kolkata and Mumbai FIRs, transponder operation is required at all times (src: notes_air_regs_vinod_yadav).
- Aircraft not given an SSR code operate Mode A code 2000 before entering the Chennai, Delhi, Guwahati, Kolkata or Mumbai FIR (src: notes_air_regs_vinod_yadav).
- Mode C continuously operated unless ATC directs otherwise (src: air_regulations_4).
- Pilot losing two-way communications sets transponder Mode A code 7600 (src: air_regulations_4).
- Unlawful interference: Mode A code 7500 (src: air_regulations_4, zenithaviation_regsnotes).
- Distress/emergency: Mode A 7700 (src: zenithaviation_regsnotes, air_regulations_4).
- Pilots shall not operate the IDENT feature unless requested by ATC (src: air_regulations_4, zenithaviation_regsnotes).
- Acknowledging mode/code setting: read back the mode and the code to be set (src: air_regulations_4, zenithaviation_regsnotes).
- Interception: aircraft equipped with transponder selects Mode A 7700 unless otherwise instructed by ATS (src: air_regulations_4).
- Intercepted crew establish radio contact on 121.5 MHz; if no contact, repeat on 243 MHz (src: air_regulations_4).
- Abrupt 90 degree (or more) climbing turn without crossing the intercepted aircraft's line of flight means "You may proceed" (src: air_regulations_4).
- Intercepted aircraft descends or lands: "DESCEND" for descend for landing; "CAN NOT" if common language not possible (src: air_regulations_4).
- Communication failure in VMC: continue in VMC, land at the nearest suitable aerodrome, report by most expeditious means (src: notes_air_regs_nirmal_firosh, air_regulations_4).
- Communication failure in IMC: squawk 7600; maintain last assigned speed and level for 20 minutes (non-radar) or 7 minutes (radar); descend at EAT; land within 30 minutes of ETA (src: notes_air_regs_vinod_yadav, notes_air_regs_nirmal_firosh, zenithaviation_regsnotes).
- Radar-environment comm failure: 7 minutes after last assigned level is reached, or after 7600 is set, or after missing a compulsory reporting point, whichever is later (src: notes_air_regs_vinod_yadav).
- Non-radar comm failure: 20 minutes after failure to report over the last compulsory reporting point (src: notes_air_regs_vinod_yadav).
- Radar identification without SSR: pilot may be asked to execute one or more heading changes of 30 degrees or more (src: air_regulations_4).
- Mode C derived level accepted as "maintaining assigned level" within +/- 300 ft of assigned level (src: air_regulations_4).
- Mode C transponder accuracy 300 ft (src: zenithaviation_regsnotes).
- Pilots of SSR-equipped aircraft: display complete call sign with pressure altitude or FL, speed and mode emergency (src: zenithaviation_regsnotes).
- ATIS is a voice broadcast; it is never transmitted on the voice channel of an ILS (src: air_regulations_4, notes_air_regs_nirmal_firosh).
- ATIS can be on a discrete VHF frequency or on the voice channel of a VOR (src: notes_air_regs_nirmal_firosh).
- ATIS broadcast message should not exceed 30 seconds where practicable (src: air_regulations_4, notes_air_regs_nirmal_firosh).
- ATIS is updated upon receipt of any official weather regardless of content change; immediately on significant change (src: air_regulations_4, notes_air_regs_nirmal_firosh).
- Preparation and dissemination of ATIS is the responsibility of the air traffic services (src: air_regulations_4).
- Heavy (for call signs): aircraft of 136,000 kg or more certified take-off mass; Light: under 136,000 kg and above 7,000 kg (src: zenithaviation_regsnotes).
- Emergency frequencies: 121.5 MHz and 243.0 MHz (international VHF/UHF distress frequencies) (src: notes_air_regs_vinod_yadav, air_regulations_fair).
- An ATS unit may ask an aircraft to temporarily change its call sign for safety reasons when there is a risk of confusion between two or more similar call signs (src: air_regulations_4).
- Heavy aircraft: the wake turbulence category "Heavy" is included immediately after the call sign (src: air_regulations_4).
- Flight plan item 10 (equipment) transponder letter: "C" = transponder Mode A (4096 codes) and Mode C (src: notes_air_regs_vinod_yadav).

## Frequently Tested Concepts

- **Mode vs code**: "Mode A" carries the code; "Mode C" carries the pressure altitude as well. Pilots read back both mode and code. (src: zenithaviation_regsnotes, air_regulations_4)
- **Special codes**: 7700 emergency, 7600 communications failure, 7500 unlawful interference. Their order is not interchangeable. (src: zenithaviation_regsnotes, air_regulations_4)
- **Interception procedures**: 121.5 MHz first (243 MHz if no contact), squawk 7700, follow intercepting aircraft instructions and ATC clarification, abrupt 90 degree climbing turn means "you may proceed". (src: air_regulations_4, zenithaviation_regsnotes)
- **Radio failure in IMC**: 7600 plus last speed/level for 20 min (non-radar) or 7 min (radar), descend at EAT, land within 30 min of ETA. (src: notes_air_regs_vinod_yadav, notes_air_regs_nirmal_firosh)
- **Radar identification**: heading change of 30 degrees or more (without SSR); "radar contact" meaning. (src: air_regulations_4, zenithaviation_regsnotes)
- **Read-back**: pilots read back the mode and the code (src: air_regulations_4).
- **IDENT**: only when requested by ATC (src: air_regulations_4).
- **ATIS**: 30 seconds, 5 NM / 5000 ft, not on ILS voice, updated on official weather change (src: air_regulations_4, zenithaviation_regsnotes).

## Numerical Problems

| Item | Value | Source |
|---|---|---|
| SSR Mode A codes available | 4096 | notes_air_regs_vinod_yadav |
| Emergency / Radio failure / Unlawful interference | 7700 / 7600 / 7500 | zenithaviation_regsnotes |
| Intercepted aircraft: first contact | 121.5 MHz (then 243 MHz if no contact) | air_regulations_4 |
| Abrupt climbing turn for "You may proceed" | 90 degrees or more | air_regulations_4 |
| Radar ID by heading change (no SSR) | 30 degrees or more | air_regulations_4 |
| Mode C assigned level tolerance | +/- 300 ft | air_regulations_4 |
| Mode C transponder accuracy | 300 ft | zenithaviation_regsnotes |
| Radio failure, radar environment: hold last level/speed | 7 minutes | notes_air_regs_vinod_yadav |
| Radio failure, non-radar: hold last level/speed | 20 minutes | notes_air_regs_vinod_yadav |
| Landing deadline after comm failure | within 30 minutes of ETA | notes_air_regs_vinod_yadav |
| ATIS broadcast length | not exceed 30 s (where practicable) | air_regulations_4 |
| ATIS range | 5 NM and 5000 ft | zenithaviation_regsnotes |
| Heavy aircraft (take-off mass) | 136,000 kg or more | zenithaviation_regsnotes |
| Light aircraft | < 136,000 kg and > 7,000 kg | zenithaviation_regsnotes |

## Memory Questions

These are real pool questions (`previous_questions/AirRegulations/CommunicationsRT.md`), copied verbatim. Every CommunicationsRT answer shown below is `derived` (model-worked key, NOT an official DGCA key). Each includes a source check.

**Q3** (Source: reg_indigo_2__flow, Confidence: derived, pool key: A)
The pilot of an aircraft losing two-way communications shall set the transponder to Mode A Code:
- A. 7600.
- B. 2000.
- C. 7500.
- D. 7700.
Check: matches "Mode A code 7600" for loss of two-way communications (src: air_regulations_4, notes_air_regs_vinod_yadav).

**Q4** (Source: 1_air_regs_question_bank_with_answers, Confidence: derived, pool key: C)
Emergency VHF frequency is
- A. 118.6 MHz
- B. 122.7 Mhz
- C. 121.5 MHz
- D. 127.0 MHz
Check: 121.5 MHz is the international VHF distress frequency (src: notes_air_regs_vinod_yadav, air_regulations_fair).

**Q15** (Source: reg_indigo_2__flow, Confidence: derived, pool key: A)
An aircraft intercepted by another aircraft, if equipped with SSR transponder shall, unless otherwise instructed by the appropriate ATS unit, select one of the following code on mode ""A""
- A. 7 700
- B. 7 500
- C. 7 600
- D. 7 000
Check: intercepted aircraft selects Mode A 7700 unless ATS instructs otherwise (src: air_regulations_4).

**Q20** (Source: reg_indigo_2__flow, Confidence: derived, pool key: A)
When acknowledging mode/code setting instructions, pilots shall:
- A. Read back the mode and code to be set.
- B. Use only the word ROGER.
- C. Use only the word WILCO.
- D. Read back only the code to be set.
Check: pilots read back the mode and the code to be set (src: air_regulations_4, zenithaviation_regsnotes).

**Q21** (Source: reg_indigo_2__flow, Confidence: derived, pool key: A)
Your transponder code assigned by ATC is 5320.In flight, in case of radio communications failure, you will squawk code :
- A. A 7600 Mode C
- B. A 5300 Mode C
- C. A 7620 Mode C
- D. A 0020 Mode C
Check: radio failure is 7600 regardless of assigned code; source answer key shows "A 7600 Mode C" for this same stem (src: air_regulations_4).

**Q25** (Source: reg_indigo_2__flow, Confidence: derived, pool key: A)
Which code shall be used on mode ""A"" to provide recognition of an emergency aircraft?
- A. Code 7700.
- B. Code 7500.
- C. Code 7600.
- D. Code 7000.
Check: Distress/emergency is 7700 (src: zenithaviation_regsnotes, air_regulations_4).

**Q29** (Source: reg_indigo_2__flow, Confidence: derived, pool key: A)
The tolerance value used to determine that mode C derived level information displayed to the controller is accurate shall be:
- A. +/- 300 ft.
- B. +/- 200 ft.
- C. +/- 250 ft.
- D. +/- 500 ft.
Check: SSR Mode C level is "within +/- 300 ft of the assigned level" (src: air_regulations_4).

## Common Mistakes

- **Radio failure vs emergency codes**: 7600 = communication failure; 7700 = emergency/distress; 7500 = hijack/unlawful interference (src: zenithaviation_regsnotes). Do not use 7700 for lost comms (the 7700 distress code is for emergency).
- **Radio failure code vs assigned code**: the assigned code is not kept for comms failure; the pilot sets 7600 (src: air_regulations_4, notes_air_regs_vinod_yadav). Pool options that show "5300" or "7620" are not the source code.
- **Mode A vs Mode C**: Mode A gives the code only; Mode C adds pressure altitude (src: zenithaviation_regsnotes). The flight plan letter "C" means Mode A and Mode C (src: notes_air_regs_vinod_yadav).
- **Read back**: read back the mode and the code, not just the code (src: air_regulations_4, zenithaviation_regsnotes).
- **Intercept frequency**: 121.5 MHz first; 243 MHz only if no contact (src: air_regulations_4). Do not treat 243 MHz as the first choice.
- **IFR communication failure timing**: 7 minutes applies in radar; 20 minutes applies in non-radar (src: notes_air_regs_vinod_yadav). Do not mix them.
- **IDENT**: pressed only when ATC asks (src: air_regulations_4, zenithaviation_regsnotes). Do not press IDENT on your own to signal a fault.
- **ATIS vs ILS voice**: ATIS is never on ILS voice channel; it may be on a discrete VHF frequency or on a VOR voice channel (src: notes_air_regs_nirmal_firosh).
- **Heavy vs Light**: 136,000 kg is the Heavy threshold; Light is above 7,000 kg and below 136,000 kg (src: zenithaviation_regsnotes).
- **Radar heading change**: 30 degrees or more (air_regulations_4). Pool options with 10 or 20 degrees are not the source figure.

## Revision Summary

- Lost comms (IFR): squawk 7600; hold last speed/level for 20 min (non-radar) or 7 min (radar); land within 30 min of ETA. (src: notes_air_regs_vinod_yadav, notes_air_regs_nirmal_firosh)
- Lost comms (VMC): continue VMC and land at nearest suitable aerodrome; report arrival by fastest means. (src: notes_air_regs_nirmal_firosh)
- Codes: 7700 emergency, 7600 radio failure, 7500 unlawful interference. (src: zenithaviation_regsnotes)
- Transponder: operate at all times in flight; Mode C continuously unless ATC directs otherwise; IDENT only on ATC request. (src: air_regulations_4)
- Read back mode and code. (src: air_regulations_4)
- Interception: 121.5 MHz (243 MHz fallback), squawk 7700, abrupt 90 degree climbing turn = "you may proceed". (src: air_regulations_4)
- Radar ID without SSR: heading change of 30 degrees or more. (src: air_regulations_4)
- Mode C tolerance: +/- 300 ft. (src: air_regulations_4)
- ATIS: voice broadcast, within 5 NM and 5000 ft, <= 30 s, never on ILS voice, updated on official weather change. (src: zenithaviation_regsnotes, air_regulations_4)
- Heavy: 136,000 kg or more; Light: under 136,000 kg, above 7,000 kg. (src: zenithaviation_regsnotes)
