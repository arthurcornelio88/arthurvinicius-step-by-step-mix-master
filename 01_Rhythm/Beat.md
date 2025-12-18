# Beat Processing Logic

## 1. Objective
Enhance the punch of the consolidated MPC drum track (Kick/Snare/Hats) and control the harmonic energy of the internal pitched sub-basses.

## 2. Technical Chain (ReaEQ + ReaComp)

| Stage | Plugin | Settings | Logic |
| :--- | :--- | :--- | :--- |
| **01 - EQ** | **ReaEQ** | **Sub-Cut:** 25Hz HPF. **Punch:** +2dB at 60Hz. **Snap:** +3dB at 3kHz. | Cleans sub-mud; emphasizes the kick "thump" and the snare "snap." |
| **02 - Dynamics** | **ReaComp** | **Ratio:** 4:1. **Attack:** 15ms. **Release:** 100ms. | The slow attack (15ms) allows the kick and snare peaks to pass through before the compressor clamps down. |

## 3. Engineering Note: Internal Sub-Basses
* Since the beat contains "pitched sub-basses," avoid aggressive high-shelving.
* If the sub-basses overlap with the main **Bassline**, use a narrow EQ dip at the specific pitch frequency if masking occurs.
