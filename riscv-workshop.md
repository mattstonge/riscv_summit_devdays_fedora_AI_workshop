# Getting Started with RISC-V, Fedora, and AI
A hands-on workshop

[BACK to HOMEPAGE](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/README.md)



## Overview

In this exercise, we will install a new operating system by installing a microSD card that has been previously flashed with an aapropriate image for this hardware based upon Fedora 42 for RISC-V.

## Materials

Your workspace will contain either a DC ROMA II laptop or desktop (both leverage the same motherboard), a freshly flashed microSD card with Fedora 42, along with torx bit screwdriver and a smudger.

![DC Roma II Laptop](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-start.jpg)

## DEMO One:

In this demo, Matt will walk everyone through flashing the microSD card with the latest image for Fedora 42/DC Roma II.
> Please Note:  You can also follow along the demo with the slide deck.

## DEMO Two:  
In this demo, Matt will walk everyone through the steps required to install the new microSD card into the DC Roma II laptop.
> Please Note:  You can also follow along the demo with the slide deck.

## DEMO Three: (optional)
In this demo, Matt will walk everyone through the steps required to install the new microSD card into the DC Roma II desktop.
> Please Note:  You can also follow along the demo with the slide deck.

## EXERCISE One (A):
Since we have flashed the microSD cards in advance (for time saving measures), we'll jump straight into installation of the microSD card into your laptop. 
> For Desktop Users - go to EXERCISE One (B): 

> Please Note: If at any time during the exercise, you have difficulty or a question - please raise your hand.


## Steps:



### 1. Ensure power OFF
> Power should already be off but if on shutdown the machine either via command line or the Graphical Desktop.
![Power supply, all cords disconnected - POWER is OFF](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-power-off.jpg)


### 2. Unplug power supply
> Disconnect the USB-C powersupply cable

### 3. Remove all modules from both sides
> While pressing the button between the slots, gently slide the modules outward.
![Remove Modules](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-release-modules.jpg)


### 4. Unscrew bottom section from the keyboard
> On the bottom of the laptop there are 5 screws. unscrew them with the torx bit.
> Please Note: The screws will NOT come all the way out - this is by design so they do not get lost. 
![Unsecure 5 screws](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-unsecure-screws.jpg)


### 5. Flip laptop over (open faced)
> Gently flip the laptop over and carefullt open it's screen, laying it flat and open on the table.
![Open flat](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-open-flat.jpg)


### 6. Use smudger to gently pry up keyboard
> Please Note: You must use extreme caution during this step as it is easy to break the ribbon cable from the keyboard that is attached to the mainboard.
> Use the smudger to gently pry up the keyboard which is also magnetically attached. Do not just rip it up and off but only raise it a few inches. 
![Open Lid](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-open-lid.jpg)
> Just lift the keyboard high enough to gently disconnect it from the mainboard. Once you have disconnected the keyboard from the mainboard set it aside.
![Open Lid](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-disconnect-ribbon.jpg)


### 7. Disconnect battery with smudger
> Using the smudger, gently pry the battery connector off.
![Disconnect battery](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-disconnect-battery.jpg)
> Ensure the battery connector is gently disconnected
![Battery disconnected](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-batt-disconnected.jpg)

### 8. Use smudger to gently lift the metal bracket holding the microSD card
> Please Note: The card bracket is very fragile. It is on a hinge and should not be totally removed. 
> USE EXTREME CAUTION
> Gentry use the smudger to unlock the card bracket (it will swing upwards but not come off).
![Old microSD](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-old-microSD.jpg)

![Lift latch](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-lift-latch.jpg)

### 9. Remove microSD card (if present)
> If there was a microSD card in the slot, please set it aside.
![Replace card](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-remove-replace-card.jpg)


### 10. Install new Fedora 42 microSD card
> Place the Fedora 42 microSD card in the slot.

### 11. Gently close/secure bracket
> Gently close the bracket and secure the microSD card.
![Close latch](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-close-latch.jpg)


### 12. Reconnect battery
> Gently reattach the battery connector.
![Reconnect battery](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-reconnect-battery.jpg)


### 13. Reconnect and replace keyboard
> Carefully, realign the ribbon cable connector and reconnect it. 
![Align connector](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-reconnect-kb1.jpg)
![Insert connector](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-reconnect-kb2.jpg)
> Carefully, realign the keyboard in its place.
![Realign keyboard](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-replace-kb.jpg)


### 14. Close & flip laptop over
> Carefully close the laptop lid and then flip the laptop over laying it flat on the table (screws visible)

### 15. Gently tighten screws
> Gently secure the screws - do not over-tighten them as it can destroy the threading.
![Secure the 5 screws](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-secure-screws.jpg)


### 16. Replace the modules back to their slots
> Replace all modules back into the slots they were originally in.
![Replace modules](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-replace-modules.gif)


### 17. Plug-in power supply
> Plug the USB-C power cord back into a USB-C slot.

### 18. TURN ON THE POWER
> Open the laptop up and gently press the power button.
> This is the end of this exercise - do not log into the machine yet.



## EXERCISE One (B):
Since we have flashed the microSD cards in advance (for time saving measures), we'll jump straight into installation of the microSD card into your desktop.

> Please Note: If at any time during the exercise, you have difficulty or a question - please raise your hand.

## Steps:




