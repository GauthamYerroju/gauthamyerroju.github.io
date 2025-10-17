---
date: '2019-11-11 23:54 -0800'
last_modified_at: '2019-11-11 23:54 -0800'
published: true
title: Sweet 16 Macro Pad Build
---
This is a build log of the Sweet 16 macro pad by [1upkeyboards.com](https://www.1upkeyboards.com/).

**Product Page:** https://www.1upkeyboards.com/shop/keyboard-kits/macro-pads/sweet16-macro-pad-white/

I bought a bundle which was on sale ($5.50 off): https://www.1upkeyboards.com/shop/keyboard-kits/macro-pads/sweet-16-nycc-bundle/

**NOTE:** There is an [updated version called Super 16 available](https://www.1upkeyboards.com/shop/keyboard-kits/macro-pads/super-16-macro-pad/), which adds support for per-key SMD LEDs  and an LED ring for underglow.

The product page [has a build log](https://www.1upkeyboards.com/instructions-downloads/sweet-16-instructions/), but I only skimmed through it, as this should be a fairly simple build.

## Parts

The kit comes with the following parts:
* PCB
* 16 Diodes
* Reset switch
* Pro Micro
* 16 Key switches of choice (I ordered Gateron Blues for the clickety clack)
* 16 Key caps (transparent, Cherry profile)
* 4 stand offs and screws to elevate the PCB
* A 1upkeyboards sticker (which looks pretty nice)

## Build

### Step 1: Solder Pro Micro headers

Solder the included Pro Micro headers with the short part of the pins facing upwards. **Do not solder the Pro Micro yet!** The key switches need to be soldered first.

### Step 2: Solder diodes and reset switch

Solder the diodes on the back of the PCB, with the black facing the square pad. Use a flush sutter to snap off the excess pins on the other side. Solder the reset switch in the position marked on the PCB.

### Step 3: key switches

Solder the key switches. This PCB supports MX and Alps style switches, but not Kailh Choc switches. I ordered Gateron Blues to go with these, because most of my boards have silen linears, and I wanted to have some clicky switches in my collection.

### Step 4: Test/Flash Pro Micro

Before soldering the Pro Micro, it's a good idea to test that it's not dead. Connect it to a computer with a Micro USB cable, open a text editor and short pins (TODO: which ones?) with a tweezer. Some characters should be detected by the computer. If nothing shows up, maybe the Pro Micro doesn't have a firmware flashed. Use other guides on the internet to flash QMK firmware, then test again. If the board is dead, it should be evident by now. Order another Pro Micro. Once the Pro Micro is flashed and working...

### Step 5: Solder Pro Micro

Align the Pro Micro on the headers on the bottom of the PCB with the micro USB port facing outwards. Note that the micro USB port should be facing outwards, not sandwiched between the Pro Micro and the Sweet 16 PCBs. Solder the Pro Micro.

### Step 6: Put on key caps of choice

...and profit!

## TLDR

Solder Pro Micro headers (short pins facing upwards, diodes (black band facing the square pad), reset switch and key switches. Make sure the Pro Micro is not dead, and solder it too. Put on some key caps and have fun!
