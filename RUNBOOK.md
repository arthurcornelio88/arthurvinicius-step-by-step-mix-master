# Implementation Runbook: step-by-step
**Status:** 🟠 In Progress (Vocal Integration)

## 🟢 Step 1: Data Normalization (COMPLETE)
- [x] Select all items.
- [x] Normalize to **-12dB Peak** (Common Gain).
    - *Result:* Mix headroom established at -5.68dB on Master.

## 🟠 Step 2: Vocal Processing (Legacy Port)
- [x] **Track Setup:** Identify the consolidated "Lead Voice" track.
- [x] **Data Cleaning:** Insert **RX 11 Mouth De-click** at the start of the chain.
- [x] **Apply Ponta-Cabeca EQ:** Load **ReaEQ** with the 350Hz cut and 10kHz air boost.
- [x] **Apply Dynamics:** Load **ReaComp** with a 3:1 ratio to stabilize the vocal levels.

## ⚪ Step 3: Frequency Slotting & Component Processing
*Goal: Data separation and instrumental clarity.*

- [ ] **Beat:** Apply punch EQ and transient-preserving compression.
    - *Ref:* [01_Rhythm/Beat.md](01_Rhythm/Beat.md)
- [ ] **Bassline:** Execute the 80Hz "Kick Pocket" cut.
    - *Ref:* [01_Rhythm/Bassline.md](01_Rhythm/Bassline.md)
- [ ] **Rhodes:** Execute the 2kHz "Vocal Pocket" cut.
    - *Ref:* [02_Melodic/Rhodes.md](02_Melodic/Rhodes.md)
- [ ] **Synth:** Execute the 2kHz "Vocal Pocket" cut.
    - *Ref:* [02_Melodic/Synth.md](02_Melodic/Synth.md)

## ⚪ Step 4: Atmospheric Depth
- [ ] **Send to Atmos:** Route the `LEAD_VOCAL_FOLDER` to the `ATMOS_BUS` (Voxengo).
    - *Target:* -18dB send level for subtle "Pop" depth.

## ⚪ Step 5: Master "Production"
- [ ] **Limiter:** Engage iZotope Ozone Maximizer.
- [ ] **Target:** -14 LUFS (Verify with Youlean).
