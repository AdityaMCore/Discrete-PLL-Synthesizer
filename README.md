# Discrete Analog PLL CSRO-VCO Frequency Synthesizer

## What it is
Phase-locked loop built from discrete ICs demonstrating 
frequency synthesis same operation as clock PLLs in SoCs.

## Blocks
| Block | Hardware | Function |
|---|---|---|
| CSRO-VCO | 74HC04 + 2N7000 | Voltage-controlled ring oscillator |
| Phase Detector | LM339 + charge pump | Analog phase comparison |
| Loop Filter | TL072 | PI integrator + buffer |
| Divider | 74HC163 | ÷N feedback |
| Power | LM317 | Clean analog supply |

## Simulation Results
- VCTRL locks at ~820µs
- VCO oscillating confirmed
- Simulation: OrCAD Capture CIS + PSpice

## Status
- [x] OrCAD schematic complete
- [x] PSpice simulation — VCO oscillating, VCTRL locked
- [ ] Hardware build 
- [ ] Measured Kvco characterization
- [ ] LTspice CMOS transistor-level respin
- [ ] Cadence Virtuoso ADE simulation
