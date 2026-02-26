# LED-Selector-Circuit-when-motor-turns
LED Selector Circuit when motor turns
Diode Threshold Priority - LED Selector Circuit when motor turn

How It Works
This circuit illustrates how parallel branches with different forward voltage thresholds compete for current when sharing a common current-limiting resistor.
One branch contains a single green LED (Vf ≈ 2.2 V).
The other branch consists of three series silicon diodes (≈ 0.7 V each) + one red LED (Vf ≈ 1.9 V), creating a much higher total threshold (≈ 4.0 V).

With the 1 kΩ resistor in the common return path, only the green LED lights: it turns on first at the lower voltage, clamps the voltage across both parallel branches to ~2.2 V, and prevents the higher-threshold red branch from conducting (Kirchhoff's voltage law in parallel paths). The resistor drops the remaining ~9.8 V and limits current to a safe ~10 mA.
When the resistor is removed (or shorted), both branches receive the full 12 V, so both LEDs illuminate brightly (but without current limiting they risk damage).

This shows why the path with the lowest forward voltage drop always wins priority in parallel arrangements — a key concept in diode logic, steering, and threshold-based selection circuits.

<img width="1084" height="1313" alt="image" src="https://github.com/user-attachments/assets/708d1b53-34e4-4add-b776-8c97cf97a711" />
<img width="1070" height="1316" alt="image" src="https://github.com/user-attachments/assets/e7dafddd-6f0e-478e-a2eb-3498465be8d5" />
<img width="698" height="394" alt="image" src="https://github.com/user-attachments/assets/720426d8-e5b1-4920-8d5f-64c4f3330366" />
