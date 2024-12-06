# Empire Biscuit Voltage Controlled Oscillator
## Details
The Empire Biscuit VCO is a Eurorack Compatible 16HP module implementation of Thomas Henry's VCO design (details available here: https://www.birthofasynth.com/Thomas_Henry/Pages/VCO-1.html).
The module is a single-voice VCO with inputs for CV, Hard Sync, Exp FM, Lin FM and PWM, and sine, triangle, ramp and square wave signal outputs.
The module has controls for Fine and coarse frequency control, FM attenuation and pulse width.
## Transistor Temperature Control
Because of the temperature sensitivity of the PNP transistors (Q1 and Q2) used in the voltage-to-current convertor circuit, it is imperative that these two transistors are thermally matched as closely as possible. For this reason, I have located them as closely together as possible.
When mounting these transistors, I suggest that you apply a small amount of thermal paste between the flat signifier sides of each transistors case, then encase them in epoxy resin (and maybe cover them up with heatshrink to go full belts and braces).
## Front Panel and Mechanical Design
I have included my design of the front panel of the Empire Biscuit ("Empire-Biscuit_PANEL-DESIGN_V1.svg"), that shows mounting hole location and the graphical design - feel free to use this fully or as a drilling template (these are all in .svg format - I recommend using Inkscape to open and edit these).

I constructed the front panel out of aluminium sheet with the following specifications:
- Sheet thickness = 2mm
- Width = 80.9mm (16HP)
- Height = 128mm (Eurorack standard)

The design shows lines for the width of the (recommended) slots at each corner of the module. The end points of these line correspond to the external radius points of each slot. I went with a slot drill size of M2.5.

Other clearance hole sizes:
- Input/Output Receptacles = 8mm
- Pots = 6mm
## Current Rev (Uploaded)
Rev A
## Mods Required After Rev A Testing
As I have not yet completed the changes for Rev B, please implement the following mods if you would like to build it to (fully working) Rev B specifications:
- +12V and -12V should be swapped around at the IDC header - I accidentally mirrored the main input voltages from the power supply, so please make sure that these are the correct way around!
- All 3/4" jacks (input and output) require new connections - Pin 1 (shield) should be connected to GND, and Pin 2 should be the respective positive connection for each. The use of TRRS receptacles for mono connections caused some confusion here.
- For all potentionmeters, swap connections to pin 1 amd 3 around so that each control increases with clockwise rotation instead of decreasing.
