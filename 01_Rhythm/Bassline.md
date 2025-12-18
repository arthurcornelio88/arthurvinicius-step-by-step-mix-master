# Bassline Processing Logic

## 1. Objective
To provide a solid low-end foundation that supports the "Beat" without masking the Kick's fundamental frequency.

## 2. Technical Chain (ReaEQ + ReaComp)

| Stage | Plugin | Settings | Logic |
| :--- | :--- | :--- | :--- |
| **01 - EQ** | **ReaEQ** | **HPF:** 35Hz. **Pocket Cut:** -3.0dB at 80Hz. | Removes sub-low rumble and creates a "hole" for the Kick drum impact. |
| **02 - Compression**| **ReaComp**| **Ratio:** 4:1. **Attack:** 10ms. **Release:** 100ms. | Stabilizes the performance; 10ms attack allows the bass "pluck" to remain articulate. |

## 3. Implementation Notes
* **Frequency Slotting:** The 80Hz cut is the "No-Sidechain" alternative. It allows the Beat's kick to punch through the mix even without dynamic ducking.
