# Lead Vocal Processing (The "Voz Boa" Consolidation)

## 1. Objective
To create a polished, "in-your-face" pop vocal that sits comfortably within the atmospheric MPC-generated backdrop.

## 2. Pre-Processing: Comping & Cleanup
* **Consolidation:** Selected best phrases from `voz boa` and `voz boa 2`.
* **Correction:** Use **iZotope RX** (Spectral De-noise/De-click) if the live environment had any floor noise or mouth clicks.
* **Pitch:** Apply gentle pitch correction (iZotope Nectar or your preferred tuner) to ensure the modern Pop "sheen."

## 3. The iZotope Stack (Main Chain)
Place these on the consolidated "Lead Voice" track:

| Stage | Plugin | Strategy |
| :--- | :--- | :--- |
| **01 - EQ** | iZotope Neutron/Nectar | **Subtractive:** Cut mud at 200Hz-300Hz. **Addative:** High-shelf boost starting at 8kHz for "air." |
| **02 - Dynamics** | iZotope Compressor | **Parallel Compression:** Use a high ratio (4:1) with a fast attack to catch peaks, blended at 60% wet. |
| **03 - De-Esser** | iZotope Nectar | Target 5kHz - 8kHz to tame harsh "S" sounds made prominent by the high-shelf boost. |
| **04 - Exciter** | iZotope Nectar | Use "Saturn" or "Tube" mode slightly to add harmonics, helping the vocal cut through the dense Rhodes/Synth. |

## 4. The Atmosphere (Spatial)
To avoid the vocal sounding "disconnected" from the MPC tracks:
* **Bus Send:** Route to **OldSkoolVerb**.
* **Setting:** Moderate Pre-delay (~20-40ms). This keeps the vocal dry and close, while the "Atmosphere" trail starts slightly later.
* **Effect:** This creates the "Atmospheric Pop" depth without washing out the lyrics.

## 5. Engineering Note: Frequency Carving
* **Action:** Check the **Rhodes** and **Synth** tracks.
* **EQ:** Apply a wide, shallow dip (-2dB to -3dB) between **1kHz and 3kHz** on those instruments.
* **Result:** This creates a "frequency pocket" for the voice to live in, eliminating the need for complex sidechaining.
