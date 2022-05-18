Wed 18 May 14:10:33 UTC 2022

A brief apology:

This (very repository on github) is a vague attempt to do
*something* interesting with an Adafruit Grand Central M4
(ATSAMD51P20A) in the context of an adwaterandstir.com
(pre-built) kit for Altair8800 (Altair-Duino) with the -b mods
done to the front panel (change in graphics; flat paddle
toggle switches).

That kit was designed to receive an Arduino Due (SAM3X8E MCU
based target board).

There's really no explicit plan in mind - this forked
repository is to draw attention to the very idea, and
to document some local experiments done .. if any!

boards.txt:

  adafruit_grandcentral_m4.build.extra_flags

    -D__SAMD51P20A__ 
    -DADAFRUIT_GRAND_CENTRAL_M4 
    -D__SAMD51__ 
    -D__FPU_PRESENT 
    -DARM_MATH_CM4 
    -mfloat-abi=hard 
    -mfpu=fpv4-sp-d16

END.
