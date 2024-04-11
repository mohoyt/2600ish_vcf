# 2600ish_vcf

## Calibration and tuning 

Taken from [Yusynth](http://yusynth.net/Modular/index_en.html)

### V/Octave tracking:
- Turn the frequency knob to 0, turn all the control knobs to 0 (fully counter clockwise)
- Apply 0V to the V/Oct input
- Measure the voltage at the basis of Q3 (node between R46, R30 to R34), adjust T1 (low freq trimmer) in order to obtain 0V at this very node.
- Apply 1V to the V/Oct input
- Adjust T2 (v/octave trimmer) in order to measure 18.7mV at the previous node.
- Apply 0V to the V/Oct input
- Adjust T1 (low freq trimmer) in order to measure -187mV at this very node.
- After the Frequency range stting (see below) you may set the filter to oscilltion mode and slightly adjust T2 in order to achieve a good V/Octave tracking.

### Frequency range setting :
- Apply a 40Hz squarewave to one of the audio input, connect the output to an amplifier.
- Set the FREQUENCY potentiometer to 0 (fully counter clockwise)
- Adjust T1 (low freq trimmer) until no signal can be heard at the output, that's it!

## Notes and known issues
- v0.1 had an issue with an extra connection around R9, but fixable on the board by rerouting R9, cutting traces and adding a bodge wire. This is fixed in v0.2
- For the panel ensure that the silkscreen is *not* subtracted from the soldermask otherwise parts of the lines and words will be difficult to read
