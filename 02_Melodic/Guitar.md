# Guitar Processing Logic

## 1. Objective
To achieve a bright, "glassy" Fender-style clean tone that cuts through the atmospheric MPC pads while maintaining a sense of depth.

## 2. Technical Chain (The "Dreamy Clean" Stack)

| Order | Plugin | Role | Setting |
| :--- | :--- | :--- | :--- |
| **01** | **ReaVerberate** | Initial Space | Room size: 30 | Dampening: 50. |
| **02** | **JS: Delay (Floaty)** | Modulation | Delay: 342ms | Mix: 31% | Feedback: 25%. |
| **03** | **ReaEQ** | Pre-Amp Prep | Subtle HPF at 180Hz to prevent low-end "chugging." |
| **04** | **Guitar Rig (NEW)** | Amp Simulation | **Target:** Fender Twin Reverb or Deluxe Reverb model. |

## 3. Guitar Rig Configuration (Fender Emulation)
* **Amp Model:** Choose the **"Twang Reverb"** (Guitar Rig's Fender Twin emulation).
* **Settings:**
    * **Bright Switch:** ON (Critical for that pop "glass" sound).
    * **Treble:** 7.5 | **Middle:** 4.0 | **Bass:** 3.5.
    * **Cabinet:** Use a 2x12 Open Back cabinet for maximum "air."
* **Post-Amp:** Add a gentle **Limiter** inside Guitar Rig to keep the transients from peaking above -12dB.
