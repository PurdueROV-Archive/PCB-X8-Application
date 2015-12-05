# LED driver overview
- Controlled by Texas Instruments LM3409HV Buck Controller
- Steps down Application board 12V power to 6V, 0.5A max
- Output current adjustable via PWM to allow for LED dimming
- Drives two high power white LEDs

# Main considerations taken in design of the board:
	- No ground plane opposite the inductor
	- Coupling capacitors located to the chip power pins
	- Drain of PFET connected as close as possible to power inductor
	- At least 4 thermal vias located under the buck controller thermal pad

(recommendations drawn from: http://rohmfs.rohm.com/en/products/databook/applinote/ic/power/switching_regulator/converter_pcb_layout_appli-e.pdf)

# Possible changes/improvements:
	- decrease the board area