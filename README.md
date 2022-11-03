# aprs_igate_direwolf
Implementation of an aprs igate using direwolf running on a Raspberry Pi

Requirements:
1. Hardware (Raspberry Pi, sound card, radio interface) fit in one Raspberry Pi project box.
2. Minimal wiring between iGate and radio.
3. Run on a headless Raspberry Pi using either Direwolf or APRX


Bill of Materials:
1. Raspberry Pi 3B
2. Audioinjector Zero - https://www.audioinjector.net/rpi-zero
3. KQ4BX Radio Interface - https://www.ebay.com/itm/233584370396
4. Hifiberry case - https://www.amazon.com/gp/product/B016954T3I/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1
5. 3.5mm TRS Female Connectors (Qty 2)
6. 3.5mm TRS Male Connectors (Qty 2)

Notes:
The Audioinjector card was chosen because it had a small footprint and fits on top of a Raspberry Pi 3B and has both audio input and audio output (and other flavors.)
The KQ4BX Radio Interface was choosen because it is a surface mount variant of the Easy Digi radio interface and the size was small enough to fit in the case with the Audioinjector card. It is important to inspect the solder connections for this part due to quality. I needed to touch up a poor solder joint.

Wiring:

<img src="https://user-images.githubusercontent.com/17286096/199636537-4fbe3f5d-b888-4361-acca-ded7e28aa97e.png" width="300" >
