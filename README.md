**This is a guide for a simple Christmas Present, using Raspberry Pi and possibly PuTTY.**
# Purpose
The initial purpose of this project is to help children who are suffering from vision disabilities and who doesn't have access to adequate education.

# Description
This present is composed of a raspberry pi, an USB cord, a breadboard, a ribbon cable, a t-cobbler, 2 resisitors, 2 LED lights, 7 wires, and one button.
A box *could* be designed at your discretion in order to cover the wiring, and making the present more asthetically pleasing. A guide for the box that we designed would also be attached. However, the present would work **perfectly** without a box or any decorations.
The program and the parts combined would allow the present to perform the following task:
- Light & Color recognization test
- Basic math test
- Basic English test
- All test questions are at a randomized order, with LED light feedback, and clear word instructions.

**Please Note: All steps needs to be followed exactly, care needs to be taken when following those steps as electricity is involved.**

# Guide
- Gather Materials, as listed above.
- Connect the ribbon cable to both the t-cobbler and the raspberry pi, then connect the t-cobbler to the breadboard, as seen in the picture. Note here that to follow the guide, you would need to connect it from the side with bigger numbers. This doesn't have to be the case, if you are not to follow the guide. You don't **have** to follow the word guide. If you already have some experience with Raspberry Pi, you can simply follow the pictures.
- Start by powering the 3V3 rail. take a wire (preferably a short one) and connect it from the port next to _SDA_ to any one of the positive ports on the bottom rail. See picture (yellow wire). Please note, when **positive** port is discussed, the positive sign on the t-cobbler should be observed, instead of the positive sign on the breadboard, if they don't align.
- Install a button right beside the end of the t-cobbler as seen in the picture.
- Power it using a wire, connect from the bottom rail (positive side) to the bottom right side of the button, as seen in the picture.
- Take a second wire and connect it from the bottom left side of the button, to port 22 on the bottom of the t-cobbler, as seen in the picture.
- If you want, you can test the button and see if it works by using a simple program.
- Now let's work on the LED lights. Start by taking a wire and connect it from the top of the raspberry pi, port 18 to port 3a, then take a resistor and put it from port 3b to port 3c. Yes, it is going to be quite compacted, but you would need space. Then, take a LED light, preferably green, take the longer side and put it in 3d, and the other side in 2d. Lastly, connect a line from 2e to the GND port. Note here that it doesn't **have** to be on the exact port. Anything on that line is fine.
- Next let's work on the other LED light. Start by connecting a wire from port 23 on the top to 3f, take the resisitor and put it from 3g to 3h, then take a LED light, preferably red, and put the longer side into 3i, and the shorter side into 2i. Lastly, connect a wire from 2j to GND on the top, in the same line with the wire from the previous step.
- That would be it for the physicals. Connect the USB wire from the Raspberry Pi's USB port into your computer, now follow the steps on the official site for setups. Please not that setup for python in Raspberry Pi also needs to be done. It is also suggested that basic python is learned before proceeding, and preferably basic Linux as well.
- After setup, type sudo nano ChristmasPresent into the command line, which would create a new file named ChristmasPresent. Copy and paste the code from the _Program_ file into it by copying it from the outside and simply right clicking in the command line. It is suggested that before doing this step, a test run is done to see whether the buttons and lights are connected correctly.
