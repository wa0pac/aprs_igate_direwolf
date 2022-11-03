# aprs_igate_direwolf
Implementation of an aprs igate using direwolf running on a Raspberry Pi

## Requirements:
1. Hardware (Raspberry Pi, sound card, radio interface) fit in one Raspberry Pi project box.
2. Minimal wiring between iGate and radio.
3. Run on a headless Raspberry Pi using either Direwolf or APRX


## Bill of Materials:
1. Raspberry Pi 3B
2. Audioinjector Zero - https://www.audioinjector.net/rpi-zero
3. KQ4BX Radio Interface - https://www.ebay.com/itm/233584370396
4. Hifiberry case - https://www.amazon.com/gp/product/B016954T3I/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1
5. 3.5mm TRS Female Connectors (Qty 2)
6. 3.5mm TRS Male Connectors (Qty 2)

## Notes:
The Audioinjector card was chosen because it had a small footprint and fits on top of a Raspberry Pi 3B and has both audio input and audio output (and other flavors.)
The KQ4BX Radio Interface was choosen because it is a surface mount variant of the Easy Digi radio interface and the size was small enough to fit in the case with the Audioinjector card. It is important to inspect the solder connections for this part due to quality. I needed to touch up a poor solder joint.

 ## Assembly:
1. To assemble the "hat" I abutted the two boards together and used a couple of drops of hot melt glue at the board joints on both the top and bottom of the boards. This formed a package that fits above the Raspberry Pi board. I used the hot glue gun to form a standoff to support the radio interface part of the assembly. The audioinjector card is supported by the header connector.
2. Two holes were drilled into the side of the case to mount the 3.5mm TRS connectors where they would not interfere with the boards.
3. The 40 pin header was soldered to the Audioinjector card.
4. The cards were connected by soldering jumper wires between the boards according to the following wiring diagram.
5. The TRS connectors were then soldered to the board using short jumper wires according to the following wiring diagram.

## Wiring:

<img src="https://user-images.githubusercontent.com/17286096/199636537-4fbe3f5d-b888-4361-acca-ded7e28aa97e.png" width="300" >

## Finished Assembly
<img src="https://user-images.githubusercontent.com/17286096/199734887-0536608a-e6d0-4cc5-a2ba-a1de266213ad.jpg" width="300">
<img src="https://user-images.githubusercontent.com/17286096/199734898-4c9f2bdf-2bce-49d3-9ec0-0bfaf38f8ada.jpg" width="300">

## Loading OS
I installed the Raspberry OS Lite 64 using the Raspberry Pi Imager using the settings to configure the hostname, ssh, username and password, wifi settings, and locale settings.

## Install and Configure 
Follow this site to setup and configure Direwolf
https://k5eok.org/2021/01/19/aprs-digipeater-igate-with-direwolf-entry-level/

Using this setup, the GPIO pin that is used for PTT is GPIO 26.

Because I used the right channel I needed to set up both Channel 0 and Channel 1. Channel 0 is not used.

I ran into problems with receiving and needed to turn on the Capture setting in the Alsa mixer. In order to do that I needed to select the Capture setting and use the spacebar to turn it on.


