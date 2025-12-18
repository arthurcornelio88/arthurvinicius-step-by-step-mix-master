# Atmosphere Bus (Voxengo OldSkoolVerb Implementation)

## 1. Concept
A centralized FX Bus to provide shared spatial DNA for the Lead Voice, Guitar, Rhodes, and Synth.

## 2. Technical Chain (As-Built)
* **Track:** `Atmos_Bus` (Track 5)
* **Plugin:** VST3: Voxengo OldSkoolVerb
* **Routing:** Direct sends from melodic tracks; `DRY MUTE` active to ensure 100% wet output.

## 3. Parameter Configuration (Verified)
Based on the current "Atmospheric Pop" calibration:

| Parameter | Value | Engineering Logic |
| :--- | :--- | :--- |
| **Pre-Delay** | 50.0 | High separation to keep the vocal transient dry and forward. |
| **Space** | 70.0 | Defines the size of the virtual room. |
| **Time** | 2000ms | 2.0s decay; provides "Atmosphere" without mudding the beat. |
| **Width** | 75.0 | Stereo spread; keeps the center clear for Kick/Voice. |
| **Damp Hi** | 7.00K | Tames digital sizzle for a warmer, more "analog" tail. |
| **EQ Mid** | -3.0 | Surgical dip in the mid-range to prevent reverb "clash". |
| **Reverb Gain**| -6.0 | Calibrated output level for the bus return. |

## 4. UI Note: Mode Selection
In this version, specific algorithm "Modes" (Plate/Hall) are accessed via the **EDIT** button next to "DEFAULT". For this project, the **DEFAULT** mode is utilized with manual knob shaping to achieve the "Atmospheric" target.

## 5. Execution Check
- [x] `DRY MUTE` engaged? (Ensures no dry signal doubling).
- [x] Input EQ clean? (HPF/LPF verified in project).
