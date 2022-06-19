# Altair8800
Source code for Arduino Altair 8800 simulator<br>
For details about the simulator see:<br>
https://www.hackster.io/david-hansel/arduino-altair-8800-simulator-3594a6

For extending the simulator with external harware see:
https://github.com/dhansel/Altair8800-IOBus

Support for Teensy 3.6 host implemented by Dirk Herrendoerfer:
https://github.com/dherrendoerfer/altair-8800-again

Please post any questions or issues in:
https://groups.google.com/forum/#!forum/altair-duino

## Altair 8800B Features

  * Turn on the "B" mode emulation from the Config menu (STOP+AUX1 Up)
  * AUX1 Up will display the Accumulator on the DATA LEDs. 
  * AUX1 Down will set the Accumulator to the value in Switches A0-A7
  * EXAMINE+AUX1 Up/Down will access the original function. 
  * If Serial Input is enabled, the function of u/U and l/c always use the non-B versions.

TODO: Input/Output Switch:
  * AUX2 Up will Read from an input port and place the value in the accumulator. The port number is the _left_ 8 switches (A8-A16)
  * AUX2 Down will Write the Accumulator to the output port set in the _left_ 8 switches

At the moment, the Accumulator display is not quite the same as the actual Altair 8800B. The real 8800B shows the Accumulator while you hold the switch, but reverts to the value at the displayed memory location when the switch is released. We are soliciting feedback on these features on the [Altairduino Forum](https://groups.google.com/g/altair-duino), and these may change based on user feedback.
