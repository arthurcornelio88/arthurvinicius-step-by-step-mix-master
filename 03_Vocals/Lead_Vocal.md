# Lead Vocal Processing (Ponta-Cabeca Reference)

## 1. Objective
Achieve a polished vocal using the established "Ponta-Cabeca" processing chain, adapted for the single "Lead Voice" track.

## 2. Technical Chain (The "Old Ref" Method)

| Stage | Plugin | Strategy/Settings |
| :--- | :--- | :--- |
| **01 - Cleanup** | **iZotope RX 11 Mouth De-click** | Remove transient saliva/mouth clicks. |
| **02 - Tone** | **ReaEQ (Cockos)** | **HPF:** 100Hz. **Low Mid:** -3dB at 350Hz. **Air:** +2.5dB High Shelf at 10kHz. |
| **03 - Compression** | **ReaComp (Cockos)** | **Ratio:** 3:1. **Attack:** 5ms. **Release:** 100ms. Aim for 3-4dB gain reduction. |
| **04 - Space** | **OldSkoolVerb (Voxengo)** | **Mix:** 15-20% (or via Bus Send). Mode: "Clear Hall" or "Plate." |

## 3. Workflow Notes
* **Merge Validation:** Since the tracks were merged, check the transition points for phase alignment or volume inconsistencies.
* **CPU Management:** RX 11 is CPU-intensive. Apply it first, then consider "Freezing" the track if Reaper playback stutters.
