# USBCArcade
Mult-form factor arcade with USB only connection from portable device

![build](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/build1.jpg "build1")
![build](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/build2.jpg "build2")
![build](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/build3.jpg "build3")
![build](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/build4.jpg "build4")
![build](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/build5.jpg "build5")
![build](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/build6.jpg "build6")
![build](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/build7.jpg "build7")
![build](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/build8.jpg "build8")

![buttons](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Buttons1.jpg "buttons")
![buttons](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Buttons2.jpg "buttons")
![buttons](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Buttons3.jpg "buttons")
![buttons](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Buttons4.jpg "buttons")
![buttons](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Buttons5.jpg "buttons")
![buttons](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/IMG_20230616_150745.jpg "buttons")


![sound](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Sound1.jpg "sound1")
![sound](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Sound2.jpg "sound2")
![sound](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Sound3.jpg "sound3")
![sound](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Sound4.jpg "sound4")
![sound](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/Sound5.jpg "sound5")


![wiring](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/wiring1.jpg "wiring1")
![wiring](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/wiring2.jpg "wiring2")
![wiring](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/wiring3.jpg "wiring3")
![wiring](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/wiring4.jpg "wiring4")
![wiring](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/wiring5.jpg "wiring5")
![wiring](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/wiring6.jpg "wiring6")


![finished](https://raw.githubusercontent.com/khinds10/USBCArcade/main/build-images/build/wiring6.jpg "finished")



# BUTTONS - Sort below


That is similar to the controller I have (mine has extra pins for leds). The controller is for 1 player (you need 2 of them for 2 players).
It is practically a 12 button GAMEPAD.
AU (up), AD (down), AR (right), AL (left) are for a microswitch joytstick (each switch with own wires) (separate pins), or a sanwa joystick (wire harness).
K1-K4 are buttons 1 to 4,
L1, L2, R1, R2 are buttons 5 to 8 (the ones you would press with your index finger)
SE - Select button, ST - Start button (or buttons 9 and 10) K11, K12 are buttons 11 and 12

The pins are simple + / - and will work with any microswitch

It is plug & play in windows and will register as a generic gamepad. You will most likely have to configure MAME's input buttons but it's easy.


Hi.. I have a different Bosega board without led-support so I am basing my comments on that. My board identifies as "0079:0006 DragonRise Inc. Generic USB Joystick". I am assuming yours does the same.

The DragonRise USB controller is commonly used in clones of the PS3 dual shock gamepad. (with 1,2,3 and 4 corresponding to triangle,circle, cross and square.) If wired up correctly it should be correctly configured in games that support these gamepads.

I have my 8 button joystick wired up like so:

K4 K1 R1 L1
K3 K2 R2 L2

(yes, R to the left of L is the correct mapping for games like street fighter on PC and consoles as R1/R2 is used as buttons 5 and 6 on a gamepad)

The MODE switch is far from useless. It switches your joystick from providing output (not input) on axes 0 and 1 (The left analog stick) or axis 4 and 5 (the d-pad). The output on the analog stick is still discrete but provides the output on the left analog stick axes.

This is especially usefull on linux with kernels 4.4-4.8 as there is a bug in the driver that messes up the analog axes. The d-pad works as intended though.
