# Clap-Switch

The Clap Switch is an engaging hobby circuit that turns on lights with a clap sound. Despite its name, the switch can be activated by any sound of a similar pitch. The core component of this circuit is the Electric Condenser Mic, which functions as a sound sensor. The mic converts sound energy into electrical energy, which then triggers a 555 timer IC through a transistor. The 555 IC activation turns on an LED, which automatically turns off after a set period.
This simple circuit employs minimal components to achieve functionality. More complex versions of clap switches with additional components can perform similar tasks, but simplicity often requires more effort than complexity.

## How It Works

1. Initial State : The transistor is off initially as the base-emitter voltage is below 0.7V. Point A is at high potential, and so is Trigger pin 2 of the 555 IC, keeping the LED off.
2. Sound Detection : When a sound is detected by the condenser mic, it converts the sound into electrical energy, raising the potential at the transistor's base and turning it on.
3. Triggering the 555 Timer : With the transistor on, point A's potential drops, triggering the 555 IC at pin 2 (below Vcc/3). This turns on the LED connected to output pin 3 of the 555 IC through a 220-ohm resistor.
4. Timer Duration : The LED remains on for 1.1 * R1 * C1 seconds. This duration can be adjusted by changing the resistor (R1) or capacitor (C1) values.
5. Automatic Turn Off : The LED automatically turns off after the set duration as the 555 timer IC operates in monostable mode.
