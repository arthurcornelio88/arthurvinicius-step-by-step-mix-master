# Atmosphere Bus (The Global Spatial Variable)

## 1. Concept
Instead of putting reverb on every track (which consumes CPU and creates "mud"), we use a **Shared FX Bus**. This creates a cohesive "acoustic space" where all instruments coexist.

## 2. REAPER Configuration
* **Track Name:** `ATMOS_BUS`
* **Input:** Receive only (No direct audio).
* **Routing:** All melodic tracks (Guitar, Rhodes, Synth, Voice) send a portion of their signal here.

## 3. Plugin: Voxengo OldSkoolVerb
To achieve the **Atmospheric Pop** sound, we want a "Lush but Clear" profile.

| Parameter | Setting | Logic |
| :--- | :--- | :--- |
| **Mode** | Reverb / Plate | Plates work best for Pop vocals and guitars. |
| **Pre-Delay** | 30ms - 50ms | Critical. This separates the dry signal from the wash, keeping the mix punchy. |
| **Space / Time** | 2.5s - 3.5s | Long enough for "Atmosphere," but not so long it overlaps the next chord change. |
| **Damping** | Moderate | Roll off highs above 6kHz to keep the reverb "darker" than the lead vocal. |
| **Width** | 100% - 120% | Maximize the stereo field to leave the "center" open for Kick and Lead Vocal. |

## 4. The "Abbey Road" Filter Trick
Place **ReaEQ** *before* the OldSkoolVerb on this bus to clean the input:
* **High Pass Filter (HPF):** 400Hz (Removes low-end clutter).
* **Low Pass Filter (LPF):** 6kHz (Removes "cheap" digital sizzle).
* **Result:** The reverb only lives in the mid-range, leaving the sub-bass and the vocal "air" pristine.

## 5. Mix Logic (The "Dry-to-Wet" Ratio)
* **Beat:** 0% Send (Keep it dry and punchy).
* **Rhodes/Synth:** 15% Send (They already have native FX; this just "glues" them).
* **Guitar:** 30% Send (Needs more space to match the synths).
* **Voice:** 20% Send (Adjust until it feels "embedded" but legible).
