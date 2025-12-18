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

## ⚪ Step 3: Frequency Slotting (The "No-Sidechain" Fix)
- [ ] **Bass/Beat Pocket:** EQ cut -3dB at 80Hz on the Bassline.
- [ ] **Melodic Pocket:** EQ cut -2dB at 2kHz on Rhodes/Synth tracks to clear space for the voice.

## ⚪ Step 4: Atmospheric Depth
- [ ] **Send to Atmos:** Route the `LEAD_VOCAL_FOLDER` to the `ATMOS_BUS` (Voxengo).
    - *Target:* -18dB send level for subtle "Pop" depth.

## ⚪ Step 5: Master "Production"
- [ ] **Limiter:** Engage iZotope Ozone Maximizer.
- [ ] **Target:** -14 LUFS (Verify with Youlean).
