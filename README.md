# VirusTI-ButMaintained
Let's fix our broken synth!

🖐 Join the [VirusTIHackers](https://discord.gg/DNn2aDwuxY) Discord 🍄

---

## Issue Tracking 🐕

### We'll use issue tracking to document the steps that need to be taken
 - Keep issues small!
  - Roadmap will be on the README
  - Link any relevant cases in the comments
 - Document your steps!
 - Create a new issue any time you reach a roadblock

###### Something you did on your journey could be a piece of the puzzle to someone else
If it's an issue marked "solved" they're more likely to see it.

---

## ❗️DO NOT share proprietary code here❗️
but do tell us how one would access it

---
	
_This is a README seed._ I'm not sure how we want to set the roadmap up yet (might even go to Wiki)
This is just a quick brain dump

###### Want to add something? I accept PRs or ping me on Discord

---

## Access has left the chat:

- USB to VST no worky
- USB to AUDIO no worky
- Does the VST still load?

## Roadblocks:

- it's possible big sur kernel extensions are no longer a thing:
 - (info maybe: https://support.apple.com/en-us/HT211860)

- the 32 bit audio driver

## Possible paths:

- SimpleVirus USBdriver
 - what is this, is it open source?

- Add the module into the kernel with OpenCore
 - is this the audio driver? 
 - This may help some people
 - Hasn't Core Audio gone away? edit: HAL API has gone away, drivers must use CoreAudio API which Polytech driver does not
  - Are there developer docs on how to update your apps?

- talk to the audio plugin company... get hired on contract, sign nda, no-compete, offer for free if we can open source any small component of it

- track down the developers at the audio plugin company. find out _everyone_ who worked on that project... maybe some have moved on and would be more open to lending a hand

- talk to the Access... get hired on contract, sign nda, no-compete, offer for free if we can open source any small component of it

- protest on site

- decompile the audio driver

-	monitor the USB traffic
 - if we can decypher the USB traffic, creating a driver from the ground up seems like the simple solution 

- monitor traffic to the kernel with `trace`

- monitor the microcontroller traffic

- harvest instructions from chips

- translation layer

- hardware mod - note: io/limitation

- time machine
