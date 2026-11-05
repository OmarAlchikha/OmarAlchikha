Hey, I'm Omar! I'm studying Electrical Engineering at York University and currently working at De Havilland Aircraft. I like electronics, computers, and figuring out how things work. Most of my projects start because I find something interesting and want to try it myself.

At De Havilland I'm a Project Engineering Intern on the Dash 8 programs. I graduate in May 2028.

Outside of school and work I'm usually into cars (EVs and hybrids especially), gaming, or taking something apart to see how it works.

## Projects

These are personal projects. Most of them are simulation and design work so far, and each README says up front what has been simulated, what has been built and what is still planned.

**Power electronics and motor control**

- [buck-converter](https://github.com/OmarAlchikha/buck-converter): a 12 V to 5 V, 2 A switching regulator with an analog PI loop. Designed and simulated in Python; the hardware package is ready but not built yet.
- [DC-Motor-Speed-Controller-System-ID-PI](https://github.com/OmarAlchikha/DC-Motor-Speed-Controller-System-ID-PI): fits a motor model from step-response data and designs a PI speed loop from it. The pipeline has only been run on synthetic data so far.
- [Three-Phase-Inverter-PMSM-Drive-FOC](https://github.com/OmarAlchikha/Three-Phase-Inverter-PMSM-Drive-FOC): field-oriented control of a permanent-magnet motor, the way EV drives do it. Python simulation only.
- [Battery-SOC-Estimator](https://github.com/OmarAlchikha/Battery-SOC-Estimator): coulomb counting vs. an extended Kalman filter for estimating a battery's state of charge. Run on a synthetic dataset so far.
- [Hybrid-electric-powertrain-energy-management-controller](https://github.com/OmarAlchikha/Hybrid-electric-powertrain-energy-management-controller): decides how to split power between a generator and a battery in a series hybrid. Python simulation.

**Aircraft-style electrical systems**

- [Arc-fault-ground-fault-detection-for-DC-wiring](https://github.com/OmarAlchikha/Arc-fault-ground-fault-detection-for-DC-wiring): detects series arcs in DC wiring from their noise signature. Validated in simulation; the hardware is designed but not built.
- [Automatic-bus-transfer-controller](https://github.com/OmarAlchikha/Automatic-bus-transfer-controller): switches a 28 VDC bus between three sources with break-before-make. Python simulation.
- [System-health-aggregator-caution-advisory-panel](https://github.com/OmarAlchikha/System-health-aggregator-caution-advisory-panel): a small web dashboard that shows simulated faults the way a cockpit caution/advisory panel would.
- [Redundant-sensor-voting-module](https://github.com/OmarAlchikha/Redundant-sensor-voting-module): three sensors measure the same thing, and the module votes on them and rejects the bad one. Logic is unit tested on a PC (50 checks); Arduino sketch included.
- [EMC-pre-compliance-rig](https://github.com/OmarAlchikha/EMC-pre-compliance-rig): a low-cost emissions test rig plus a model that predicts how noisy the buck converter will be. Design and modeling only so far.

**Digital hardware**

- [FPGA-Digital-Control-Core-DE10-Lite](https://github.com/OmarAlchikha/FPGA-Digital-Control-Core-DE10-Lite): a PWM generator and quadrature encoder decoder in Verilog, with self-checking testbenches (23/23 passing).

I use Claude Code as a design assistant on these and work through each part myself. Everything here uses public, textbook-level engineering only. Nothing comes from my employer.

## Tools I use

C, Python, Verilog, MATLAB/Simulink, LTspice, Quartus, Icarus Verilog, Arduino, DE10-Lite

## Contact

[om.alchikha@gmail.com](mailto:om.alchikha@gmail.com) · [LinkedIn](https://www.linkedin.com/in/omaral-chikha)
