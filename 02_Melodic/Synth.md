# Synth Processing Logic

## 1. Objective
Control the stereo energy of the synth pads and ensure they wrap *around* the vocal rather than sitting on top of it.

## 2. Technical Chain (ReaEQ + ReaComp)

| Stage | Plugin | Settings | Logic |
| :--- | :--- | :--- | :--- |
| **01 - EQ** | **ReaEQ** | **HPF:** 200Hz. **Vocal Pocket:** -2.0dB at 2kHz. | Removes "mud" that conflicts with the Bassline and mirrors the Rhodes pocket for the vocal. |
| **02 - Dynamics** | **ReaComp** | **Ratio:** 2.5:1. **Release:** 200ms. | Smoother, longer release to keep the pad "Atmospheric" and steady. |

## 3. Integration
* **Slotting:** By cutting 2kHz on both Synth and Rhodes, we create a "2kHz Corridor" where the Lead Voice can sit without competition.
