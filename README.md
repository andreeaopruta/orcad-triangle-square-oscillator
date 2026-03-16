# Analog Triangle-Square Wave Generator

## Project Overview
This repository contains the comprehensive documentation for a variable-frequency, variable-amplitude analog signal generator. Designed as a Computer-Aided Design (CAD) project, the circuit produces stable and symmetrical triangular and square waveforms, with its performance verified through OrCAD PSpice simulations.

### Key Specifications
* **Power Supply:** Symmetrical ±18V.
* **Adjustable Frequency:** Configurable between 8.5kHz and 18kHz.
* **Square Wave Amplitude:** Adjustable between 5V and 9V.
* **Triangle Wave Amplitude:** Adjustable between 4V and 10V.

## Circuit Architecture
The generator relies on two primary functional blocks built around TL082 operational amplifiers:
1. **Schmitt Trigger (Comparator with Positive Feedback):** Generates the square wave signal. The amplitude is fine-tuned using a dedicated resistive voltage divider network at the output.
2. **Integrator:** Converts the square wave from the comparator into a linear triangular wave. 
3. **Control Network:** The circuit utilizes E24 series resistors and multiple potentiometers to allow independent control over the oscillation frequency and the output amplitudes.

## Repository Contents
* `Project_Documentation.pdf`: The complete design report. It includes:
  * The full OrCAD electrical schematic.
  * Mathematical design calculations for frequency and voltage dividers.
  * Component selection justifications and theoretical formulas.
  * Transient analysis waveform plots from OrCAD PSpice, demonstrating the circuit's accurate operation at both minimum and maximum thresholds.
