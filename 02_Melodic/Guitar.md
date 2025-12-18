# Guitar Processing Logic

## 1. Objective
To achieve a bright, "glassy" Fender-style clean tone that cuts through the atmospheric MPC pads while maintaining a sense of depth.

## 2. Technical Chain (The "Dreamy Clean" Stack)

| Order | Plugin | Role | Setting |
| :--- | :--- | :--- | :--- |
| **01** | **ReaVerberate** | Initial Space | Room size: 30 | Dampening: 50. |
| **02** | **JS: Delay (Floaty)** | Modulation | Delay: 342ms | Mix: 31% | Feedback: 25%. |
| **03** | **ReaEQ** | Pre-Amp Prep | Subtle HPF at 180Hz to prevent low-end "chugging." |
| **04** | **ReaComp (NEW)** | Compressor | Stabilize the input signal |
| **05** | **Guitar Rig (NEW)** | Amp Simulation | **Target:** Fender Twin Reverb or Deluxe Reverb model. |

## 3. Guitar Rig Configuration (Fender Emulation)
* **Amp Model:** Choose the **"Twang Reverb"** (Guitar Rig's Fender Twin emulation).
* **Settings:**
    * **Bright Switch:** ON (Critical for that pop "glass" sound).
    * **Treble:** 7.5 | **Middle:** 4.0 | **Bass:** 3.5.
    * **Cabinet:** Use a 2x12 Open Back cabinet for maximum "air."
* **Post-Amp:** Add a gentle **Limiter** inside Guitar Rig to keep the transients from peaking above -12dB.

## 4. Dynamics: ReaComp (Cockos)
Place this AFTER the delay but BEFORE Guitar Rig to stabilize the input signal.

| Parameter | Setting | Logic |
| :--- | :--- | :--- |
| **Ratio** | 2.5:1 | Gentle control to maintain a "natural" feel. |
| **Attack** | 10.0 ms | Allows the initial pick attack to remain "bright" before compression. |
| **Release** | 150 ms | Smoothly returns the gain, sustaining the reverb/delay tails. |
| **Threshold** | Adjust for -3dB | Target just enough reduction to even out the performance. |
