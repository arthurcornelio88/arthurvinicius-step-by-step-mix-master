# Implementation Runbook: step-by-step
**Status:** 🟢 Ready for Execution
**Version:** 1.0.0 (Rapid Mix)

This document serves as the technical roadmap for the mixing session, linking to the specific logic defined in the project documentation.

---

## 🟢 Phase 1: Data Prep & Environment Setup
*Goal: Establish headroom and a clean "source of truth."*

1.  **Vocal Comping:** Consolidate `voz boa 1` and `2` into a single "Lead" track.
    * *Ref:* [03_Vocals/Lead_Vocal.md](03_Vocals/Lead_Vocal.md)
2.  **Gain Staging:** Normalize all MPC stems and live recordings to peak at **-12dB**.
3.  **Global Routing:** Create the `ATMOS_BUS`.
    * *Ref:* [04_Busses_FX/Atmosphere_Bus.md](04_Busses_FX/Atmosphere_Bus.md)

---

## 🟡 Phase 2: Frequency Slotting (The "No-Sidechain" Fix)
*Goal: Resolve low-end and vocal masking via surgical EQ.*

1.  **Bassline vs. Beat:** Open **ReaEQ** on Bassline; carve the Kick pocket (60Hz-100Hz).
    * *Ref:* [00_Project_Specs.md](00_Project_Specs.md) (Strategy Section)
2.  **Melodic Pocketing:** Dip the Rhodes and Synth at **1.5kHz - 3kHz** to make room for the Lead Vocal.
3.  **Guitar Character:** Initialize **Guitar Rig**; focus on "Dreamy/Modulated" tones to match the Rhodes.
    * *Ref:* [02_Melodic/Guitar.md](02_Melodic/Guitar.md)

---

## 🔵 Phase 3: The Atmospheric Layering
*Goal: Merging live elements with MPC "baked" textures.*

1.  **Voxengo Deployment:** Set **OldSkoolVerb** to "Plate" mode with 30ms Pre-delay.
2.  **Dry/Wet Balance:** * Send **Guitar** to Atmos Bus at -10dB.
    * Send **Voice** to Atmos Bus at -15dB.
    * Send **Rhodes/Synth** at -20dB (Correctional glue only).
    * *Ref:* [04_Busses_FX/Atmosphere_Bus.md](04_Busses_FX/Atmosphere_Bus.md)

---

## 🔴 Phase 4: Final Compilation (Mastering)
*Goal: Achieving commercial loudness and final glue.*

1.  **Master Chain:** Engage iZotope Ozone/Neutron on the Master track.
2.  **Loudness Targeting:** Monitor via **Youlean Loudness Meter**.
    * **Target:** -14 LUFS / -1.0dB True Peak.
    * *Ref:* [04_Busses_FX/Mix_Bus.md](04_Busses_FX/Mix_Bus.md)

---

## 🏁 Deployment Checklist
- [ ] Vocal is intelligible and sits "above" the synths?
- [ ] Bass and Kick are distinct without sidechaining?
- [ ] Atmosphere is lush but doesn't wash out the "Beat" transients?
- [ ] Repository documentation updated with final EQ/Compression values?
