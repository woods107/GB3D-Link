# GB3D-Link
A "link cable" to bring together GB(C) and 3DS Virtual Console versions

This project is intended to create a communication bridge between Virtual Console and original cartridge releases of various Nintendo games. The primary focus is on enabling trading between the VC and cartridge releases of Pokemon Red/Blue/Yellow and Gold/Silver/Crystal.

GB3D-Link uses code from and based on the Citra 3DS emulator for its work on local communications, and is licensed under the GPLv2 (or any later version). Refer to the license.txt file included.

# Project goals:
* to successfully emulate 3DS local wireless communications, while minimizing the amount of other system emulation required
* to be able to broadcast/transmit and receive those communications with WiFi-capable hardware
* to successfully emulate and read GB(C) Link Cable transmissions
* to "translate" communications from GB(C) Link Cable format into 3DS local wireless format, and vice versa

# Possible complications:
* timing discrepancies in relation to hardware differences (GB to adapter hardware, adapter hardware to 3DS local wireless)
** link cable is synchronous, requires precise clock timings (Can communications be handled in stages? For example, use placeholder/dummy wireless connections to establish connection to 3DS, convert to link cable format, and begin sending data to GB *after?* Or use placeholder/dummy "filler" signal over link cable until 3DS packets are translated?)
