# Omar Alchikha

**Electrical Engineering @ York University (Lassonde)** — power electronics, embedded hardware, and the electrical systems behind aircraft and EVs.

Currently a **Project Engineering Intern at De Havilland Aircraft of Canada**, working aircraft modification and engineering configuration on the Dash 8-400 and DHC-515 programs. Graduating May 2028.

The repos here are personal project work, built on public engineering knowledge only. They run in three threads.

---

### ⚡ The powertrain series

Five projects that build on each other — each one designed against the **real measured output** of the one before it, not idealized numbers.

| | Project | What it is |
|---|---|---|
| 1 | **[buck-converter](https://github.com/OmarAlchikha/buck-converter)** | 12V→5V closed-loop converter. PI compensator derived from a state-space averaged plant, cross-validated across Python, LTspice and Simulink. |
| 2 | **[DC-Motor-Speed-Controller-System-ID-PI](https://github.com/OmarAlchikha/DC-Motor-Speed-Controller-System-ID-PI)** | Motor speed loop where the plant is *identified from a step response*, not assumed — because friction and dead time aren't on any datasheet. |
| 3 | **[Battery-SOC-Estimator](https://github.com/OmarAlchikha/Battery-SOC-Estimator)** | Coulomb counting vs. an extended Kalman filter. The EKF starts from a deliberately wrong state of charge and still beats it. |
| 4 | **[Three-Phase-Inverter-PMSM-Drive-FOC](https://github.com/OmarAlchikha/Three-Phase-Inverter-PMSM-Drive-FOC)** | Field-oriented control of a PMSM traction drive, with loop gains derived from a delay budget rather than tuned. |
| 5 | **[Hybrid-electric-powertrain-energy-management-controller](https://github.com/OmarAlchikha/Hybrid-electric-powertrain-energy-management-controller)** | Series-hybrid supervisor deciding the generator/battery power split across a flight-shaped mission. |

### ✈️ Aircraft electrical systems

Protection, monitoring, redundancy, and distribution — the systems that tell you the truth about an electrical system's state.

- **[System-health-aggregator-caution-advisory-panel](https://github.com/OmarAlchikha/System-health-aggregator-caution-advisory-panel)** — a simplified aircraft CAS panel. Sources report facts; one severity-policy table decides what gets annunciated.
- **[Automatic-bus-transfer-controller](https://github.com/OmarAlchikha/Automatic-bus-transfer-controller)** — 28 VDC three-source transfer with strict break-before-make. Includes a deliberately-wrong version to *measure* why the sequencing matters.
- **[Arc-fault-ground-fault-detection-for-DC-wiring](https://github.com/OmarAlchikha/Arc-fault-ground-fault-detection-for-DC-wiring)** — a series arc reduces current, so no breaker catches it. Detected by noise signature instead, validated against a physics-based waveform simulator.
- **[Redundant-sensor-voting-module](https://github.com/OmarAlchikha/Redundant-sensor-voting-module)** — 2-out-of-3 mid-value-select voting with graceful degradation, and a deliberate refusal to guess when it can't arbitrate.
- **[EMC-pre-compliance-rig](https://github.com/OmarAlchikha/EMC-pre-compliance-rig)** — near-field probe + LISN + SDR rig, with an emissions model that ranks mitigations before any parts are ordered.

### 🔧 Digital hardware

- **[FPGA-Digital-Control-Core-DE10-Lite](https://github.com/OmarAlchikha/FPGA-Digital-Control-Core-DE10-Lite)** — parameterized PWM generator and quadrature decoder in Verilog, with self-checking testbenches (23/23 checks) and a complete Quartus synthesis project.

---

### How I work

- **Cross-validation as a habit** — most projects carry two or three independent implementations that have to agree, sharing no code.
- **Derive, don't tune** — controller gains come from a stated crossover, phase margin, or delay budget, never from twiddling until a plot looked right.
- **Honest scope** — every repo states what's simulated, what's measured, and what's a placeholder.

**Tools:** C · Python · Verilog · MATLAB/Simulink · LTspice · Quartus · Arduino · DE10-Lite

📫 [om.alchikha@gmail.com](mailto:om.alchikha@gmail.com) · [LinkedIn](https://www.linkedin.com/in/omaral-chikha)
