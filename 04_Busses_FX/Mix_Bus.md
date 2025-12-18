# Mix Bus & Final Mastering Logic

## 1. Objective
To "glue" the atmospheric layers together and achieve commercial loudness (-14 to -12 LUFS) without destroying the transients of the MPC beat.

## 2. The Master Chain (iZotope / Cockos)

| Stage | Plugin | Logic |
| :--- | :--- | :--- |
| **01 - Glue** | ReaComp / iZotope | **Slow Attack (30ms), Fast Release.** Ratio 1.5:1. Only 1-2dB of reduction. This makes the beat and the synths feel like "one instrument." |
| **02 - Tonal EQ** | iZotope Ozone EQ | **Matching:** Compare against a reference Atmospheric Pop track. Usually requires a tiny "smile" curve (+1dB at 60Hz, +1dB at 10kHz). |
| **03 - Imager** | iZotope Ozone Imager | **Stereo Width:** Keep frequencies below 200Hz in mono. Widen the 2kHz+ range by 10-15% to enhance the "Atmosphere." |
| **04 - Maximizer** | iZotope Ozone Limiter | **Mode:** IRC IV (Modern). Target -14 LUFS for streaming. Set Ceiling to -1.0dB to prevent TP (True Peak) clipping. |

## 3. Analysis Metrics
* **Target Loudness:** -14 LUFS (Integrated).
* **Peak:** -1.0 dBFS.
* **LRA (Loudness Range):** Aim for 6-8 LU rating for Pop (keep it dynamic but controlled).
* **Tool:** **Youlean Loudness Meter** at the very end of the chain.
