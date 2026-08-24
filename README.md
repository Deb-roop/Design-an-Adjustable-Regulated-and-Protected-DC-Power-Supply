# Design-an-Adjustable-Regulated-and-Protected-DC-Power-Supply
## Adjustable, Regulated, and Protected DC Power Supply

> **Course:** ECE 2200 - Electronic Circuits Design Laboratory (Khulna University of Engineering & Technology)[cite: 1]
> **Group:** B-03[cite: 1]

### Overview and Key Features
This project features the comprehensive design, simulation, and hardware implementation of an adjustable, regulated DC power supply[cite: 1]. It efficiently converts a 230 V AC mains supply into a continuously variable DC output ranging from 1.25 V to 30 V[cite: 1]. To safeguard connected loads from electrical faults, it integrates a fast-acting MOSFET crowbar cutoff mechanism paired with operational amplifier comparators[cite: 1]. 

*   **Adjustable Output:** Utilizes the LM338K active linear voltage regulator for smooth and continuous voltage adjustments[cite: 1].
*   **Over Voltage Protection (OVP):** Automatically isolates connected loads whenever the output voltage exceeds safe operational limits[cite: 1].
*   **Under Voltage Protection (UVP):** Disconnects loads when the supply drops below a minimum threshold to prevent erratic circuit behavior[cite: 1].
*   **Short Circuit Protection (SCP):** Uses a 2N7000 MOSFET crowbar cutoff switch to rapidly suppress excessive current surges without mechanical contact bounce[cite: 1].
*   **Visual Indicators:** Integrates Red and Green status LEDs for real-time monitoring of normal power delivery and fault states[cite: 1].

---

### Core Governing Equations
The mathematical foundation of the power supply design relies on standard rectification, filtering, and active regulation principles[cite: 1]:

*   **Peak Rectified Voltage:** $V_{peak}=V_{RMS}\times\sqrt{2}-2\times V_{D}$[cite: 1]
*   **Capacitive Ripple Voltage:** $V_{ripple(p-p)}=I_{load}/(f_{ripple}\times C1)$[cite: 1]
*   **Adjustable Output Voltage:** $V_{out}=V_{ref}\times(1+RV1/R1)+I_{adj}\times RV1$[cite: 1]

---

### Experimental Performance Results
The unified system was successfully validated through Proteus ISIS software simulations and physical solderless breadboard testing over a minimum load resistance of 330 Ω[cite: 1].

| Performance Parameter | Simulation (Proteus ISIS) | Hardware Breadboard |
| :--- | :--- | :--- |
| Adjustable Voltage Range | 0.78 V - 28.2 V[cite: 1] | 1.1 V - 28.7 V[cite: 1] |
| OVP Threshold | 26.1 V[cite: 1] | 22.5 V[cite: 1] |
| UVP Threshold | 5.42 V[cite: 1] | 3.3 V[cite: 1] |
| Maximum Power Output | 1.42 W[cite: 1] | 0.94 W[cite: 1] |
