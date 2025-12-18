# Mix Bus & Final Mastering Logic (Legacy Port)

## 1. Objective
To "glue" the atmospheric layers together, add analog-style saturation, and achieve commercial loudness targets using the established legacy plugin chain.

## 2. The Master Chain (Refactor)

| Order | Plugin | Role | Setting/Strategy |
| :--- | :--- | :--- | :--- |
| **01** | **FerricTDS** | Tape Dynamics/Saturation | **Drive:** +1.0 dB. Adds harmonic "glue" and tames transients smoothly. |
| **02** | **TDR Nova** | Dynamic EQ | **Tonal Balance:** Gentle adjustments (±2 dB max) to polish the final spectrum. |
| **03** | **LoudMax** | Lookahead Limiter | **Output:** -1.0 dBTP. Adjust **Threshold** to hit the LUFS target. |
| **04** | **Youlean Loudness Meter** | Analysis | Final verification of Integrated LUFS and True Peak. |

## 3. Technical Targets
* **Streaming (YouTube/Spotify):** -14 LUFS Integrated.
* **Peak Ceiling:** -1.0 dBTP (True Peak) to prevent distortion during platform transcoding.
* **Dynamics:** Monitor the Loudness Range (LRA) to ensure the "Atmospheric" breath is preserved.

## 4. Execution Notes
* **FerricTDS:** Use this to add "weight" to the MPC beat and the low-end.
* **TDR Nova:** Focus on the 2kHz - 5kHz range if the vocal or guitar feels too "piercing" at high volumes.
* **LoudMax:** The primary tool for loudness. Ensure the gain reduction meter isn't constantly pinned; aim for transparent limiting.

## 5. Advanced Dynamics (FerricTDS mkII)
* **High-End Smoothing:** Used as a global de-esser for the "Atmosphere" by pushing Saturation to 25%.
* **Transient Glue:** Dynamics knob set to 30% to pull the Kick/Snare peaks into the instrumental bed.
* **Recovery:** Set to "Fast" to maintain the "step-by-step" rhythmic urgency.
