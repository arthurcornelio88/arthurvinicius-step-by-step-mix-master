# Implementation Runbook: step-by-step
**Status:** 🟠 In Progress (Vocal Integration)

## 🟢 Step 1: Data Normalization (COMPLETE)
- [x] Select all items.
- [x] Normalize to **-12dB Peak** (Common Gain).
    - *Result:* Mix headroom established at -5.68dB on Master.

## 🟠 Step 2: Vocal Architecture (CURRENT TASK)
- [x] **Create Folder:** Create `LEAD_VOCAL_FOLDER` and move `voz boa` & `voz boa 2` inside.
- [x] **Handle Overlaps:** Check the transitions at [1:36.000]. Use 50ms crossfades where phrases overlap.
- [ ] **iZotope Chain:** Load the processing chain on the **Folder Track** (not the individual tracks).
    - *Technical Details:* See [03_Vocals/Lead_Vocal.md Section 3]

## ⚪ Step 3: Frequency Slotting (The "No-Sidechain" Fix)
- [ ] **Bass/Beat Pocket:** EQ cut -3dB at 80Hz on the Bassline.
- [ ] **Melodic Pocket:** EQ cut -2dB at 2kHz on Rhodes/Synth tracks to clear space for the voice.

## ⚪ Step 4: Atmospheric Depth
- [ ] **Send to Atmos:** Route the `LEAD_VOCAL_FOLDER` to the `ATMOS_BUS` (Voxengo).
    - *Target:* -18dB send level for subtle "Pop" depth.

## ⚪ Step 5: Master "Production"
- [ ] **Limiter:** Engage iZotope Ozone Maximizer.
- [ ] **Target:** -14 LUFS (Verify with Youlean).
