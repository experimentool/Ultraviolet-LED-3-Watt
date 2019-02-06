# Ultraviolet-LED-3-Watt
This repository is not a programming type at this point.  It shows how to power a 3 watt LED without using a constant current LED driver.
The LED wavelength is 395-405 nm.  The light emitted will be used to search for luminescent rocks such as sodalite. 
I am using 2 lipo 18650 cells in series to power the circuit.  I have them configured as a 2S pack with a jxt-xh 3 pin connector to make 
the cells easier to charge with a commercial lipo charger.
The positive voltage output of the 2S pack goes through a single pole single throw toggle switch and a 1N5408 silicon diode before 
connecting to a mini 360 buck converter.  The mini 360 has been modified by removing the potentiometer that is very inadequate.
The pot is replaced by a resistance of approximately 28.8k that gives an output of 3.95 volts from the mini 360.
A DC current of 500-550 mA is applied to the 3W LED at 3.95 volts.
I am using unprotected 18650 cells so a 800 mA fast blow fuse has been added to the negative leg of the DC power.
The cells are also protected from low voltage by the 1N5408 voltage drop of 0.7V and the low voltage cutoff provided 
by the 3W LED turning off below 2.5V.  So when the cell voltage gets below 3.0 - 3.2 V the current in this part of the circuit falls
rapidly therby protecting the cells from discharging to an unsafe voltage.
The red LED and the temperature switch are to let the operator know that it may be time to switch off to allow the 3W LED to cool.
