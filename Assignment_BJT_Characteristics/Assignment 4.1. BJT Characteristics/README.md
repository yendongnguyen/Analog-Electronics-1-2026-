Dong Nguyen

Objective

The objective of this assignment is to simulate and analyze the input-output characteristics of an NPN BJT (2N2222) using LTspice. The goal is to observe the relationship between collector current (IC) and base current (IB), estimate the DC current gain (β = IC/IB), and analyze the output characteristics (IC vs VCE).

Part A – Transfer Characteristic (IC vs IB)

The emitter was connected to ground, the collector to a 10 V DC supply, and the base was driven by a DC current source.
Base current was swept using: .dc I1 0 1m 1u
Collector current increased approximately linearly with base current in the active region.

β was calculated using:
β = IC / IB
Measured Values
IB = 0.1 mA → β ≈ 180
IB = 0.5 mA → β ≈ 170
IB = 1.0 mA → β ≈ 150
β decreases slightly as IC increases.
Output Characteristic (IC vs VCE)
VCE was swept using: .dc V1 0 10 0.1
Base current was stepped: .step param IB list 0.1m 0.5m 1m
In the active region, IC remains almost constant with increasing VCE.
At low VCE, the transistor enters saturation, and IC decreases.

Part B
The IC–IB relationship is approximately linear in the active region. The collector current increases proportionally with the base current. However, the slope is not perfectly constant, indicating that β slightly changes as the collector current increases.

IC is approximately proportional to IB in the active region.
From the simulation:
At IB = 0.1 mA, β ≈ 180
At IB = 0.5 mA, β ≈ 170
At IB = 1.0 mA, β ≈ 150
The results show that β decreases slightly at higher current levels
The 10 V supply keeps the transistor in the active region. If VCE is very small, the transistor saturates and gain decreases.


Conclusion
The simulation confirms that IC is controlled by IB in the active region. The current gain β is not constant and slightly decreases at higher currents. The output curves clearly show active and saturation regions.
