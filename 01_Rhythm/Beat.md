# Beat Processing Logic

## 1. Objective
To maintain the integrity of the MPC consolidated drums while ensuring the "pitched sub-basses" do not muddy the low-end or clash with the main Bassline.

## 2. Technical Chain (ReaEQ + ReaComp)

| Stage | Plugin | Settings | Logic |
| :--- | :--- | :--- | :--- |
| **01 - EQ** | **ReaEQ** | **HPF:** 30Hz. **Kick Punch:** +2dB @ 60Hz. **Snare Snap:** +3dB @ 3kHz. | Cleans subsonic noise; emphasizes the fundamental thump and high-end definition. |
| **02 - Dynamics**| **ReaComp**| **Ratio:** 4:1. **Attack:** 15ms. **Release:** 100ms. | Slow attack allows transients (Kick/Snare) to pass before compression kicks in. |

## 3. Handling Pitched Sub-Basses
* Since the beat includes melodic low-end, use a narrow EQ dip if a specific note resonates too loudly or clashes with the Bassline track.
