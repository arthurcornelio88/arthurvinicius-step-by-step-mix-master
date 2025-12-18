# Rhodes Processing Logic

## 1. Objective
Maintain the atmospheric "warmth" of the MPC native effects while clearing the "presence" range for the Lead Vocal.

## 2. Technical Chain (ReaEQ + ReaComp)

| Stage | Plugin | Settings | Logic |
| :--- | :--- | :--- | :--- |
| **01 - EQ** | **ReaEQ** | **LPF:** 12kHz. **Vocal Pocket:** -2.0dB at 2kHz (Wide Q). | Removes "MPC sizzle" and clears the primary intelligibility range for the voice. |
| **02 - Dynamics** | **ReaComp** | **Ratio:** 2:1. **Threshold:** Gentle. | Acts as a "leveler" to prevent the Rhodes from jumping ahead of the vocals during loud chords. |

## 3. Atmospheric Note
* **Native FX:** Respect the baked-in MPC reverb/chorus. This EQ comes *after* those effects to shape the final output.
