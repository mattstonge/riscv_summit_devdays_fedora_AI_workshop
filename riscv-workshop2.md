# Optimizing Fedora
A hands-on workshop

[BACK to HOMEPAGE](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/README.md)



## Overview
Now, we will install addtional packages, optimize the desktop and tune the systems in preparation for the setup of our AI environments.

## DEMO One: 
Matt will demo the multiple steps to enhance, tune and optimize the Fedora 42 environment in preparation for the AI installations.
![DC Roma II Laptop](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-start.jpg)



> 


--------------------------------------------------------

## Hands-on Exercise One:
**Overview:**  In this exercise we will shape and tune Fedora to optimally run AI. This part is hardware agnostic - the steps are the same for the desktop systems and the laptops.

### Steps: 

#### 1. Initial login
> log into the laptop with the default user "roma" and password "roma".
![Gnome Login](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-gnome-login.jpg)


#### 2. Configure network
> CLick on the upper right-hand corner of the screen to bring up the settings.
Select: WIFI (by clicking on the side arrow next to "WIFI")
![WIFI Menu access](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-WIFI1.png)

A list of available WIFI hotspots will appear
Select: (We'll let you know which one to connect to)
![SSID Selection](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-WIFI2.png)
Enter the WIFI passphrase: (TBD)
> information for the network configuration will be provided.
> 

#### 3. Configure Date/Time
> Open the Settings menu

> Scroll down and Select: System
![System Menu](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-daytime1.png)

> Select: Date & Time
![Date Time Options](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-daytime2.png)

> Activate: Automatic Time Zone & Clock & Calendar: Weekday by clicking on the activation switch.
![Enable Date Time options](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-daytime3.png)

> exit Settings
>

#### 4. Disable Bluetooth
> Disabling Bluetooth as it's not needed - and anything not needed should be disabled for security reasons.
> Click on the upper right hand corner to engage the settings panel.
![See BT](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-BT1.png)

> Click on the "Bluetooth" button (this is a switch that can enable/disable - we don't need to open the full settings dialog)
![BT off](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-BT2.png)

> 


#### 5. Custom workshop repository configuration
> information will be provided (if other than provided by what's configured in the image)

> 


#### 6. Initial package installation
> Open a terminal session
``` 
$  sudo -i
(enter roma password when prompted)

#  dnf install -y gnome-tweaks 
(output omitted)


#  dnf install -y info btop

# exit

$ gnome-tweaks


```

> We'll now use the gnome-tweaks application to ensure the minimize and maximize buttons are added to all windowsd within the Gnome Desktop envionrment.
![tweaks launch](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-tweaks1.png)
> Click "OK" to continue...
> In the left menu - Select "Windows"
![tweak selection1](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-tweaks2.png)


![tweak window options](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-tweaks3.png)


![Tweaks selected](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-tweaks4.png)
> Once you select (Activate) Maximize & (Activate) Minimize - exit the application.
> You can also exit the terminal window as well...

```

$ exit 

```

> 


#### 7. Online resizing of the root volume
> In this exercise we will do an online resizing of the ROOT volume so as we have enough diskspace to update Fedora, add more applications and eventually add some AI models.

**PLEASE NOTE: On some machines the Fedora First Boot sequence may have already done this behind the scenes.**
**To test if you need to resize - run "df -h" in a terminal - if root ( / ) is not greater than 200GB - you need to execute this exercise.**

> First, click on the bar in the upper left hand corner, and then click on the box of 9 dots at the bottom of the screen - this will show a screen with installed applications to choose from.

![Disks 1](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-disks1.png)

> Click on the "Utilities application group"
![Disks 2](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-disks2.png)

> Click on "Disks"
> What appears next is the filesystem layout on the microSD card where Fedora 42 is installed.
![Disks 3](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-disks3.png)

> Click on the volume called "root" 
![Disks 4](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-disks4.png)

> Click on the gear box to bring up the options menu
![Disks 5](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-disks5.png)

> Click on "Resize"
![Disks 6](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-disks6.png)

> Move the slider all the way to the farthest point on the far right.
![Disks 7](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-disks7.png)

> Click the red RESIZE button.
> Once the spinning disc has stopped (and disappears) the resize operation is complete and you may exit gnome-disks.
![Disks 8](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-disks8.png)

> OPTIONAL - you could open a terminal and perform a "df -h" to verify the resize.
![Disks 9](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-disks9.png)




--------------------------------------------------------






## DEMO Two
Matt will walkthrough how to optimize the system in preparation for the AI applications installation.

## Hands-on Exercise Two:

### STEPS: 

#### 1. Systems settings deep dive
> In the previous exercises we installed a tool called "btop". Open a terminal session.

```

$  btop

```

![btop 1](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-btop1.png)
> You can now exit BTOP by pressing "q" or by closing the terminal.




#### 2. Power Management
> In this exercise, we will confirm Power Management settings are set to give the system the highest performance values.
> Open up the Settings main menu and Select: Power


![Power 1](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-power1.png)


> Click on Show Battery Percentage - and a new Battery indicator will appear in the top bar.
![Power 2](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-power2.png)



> Click on the Power Saving tab and more options will appear.
![Power 3](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-power3.png)



> Disable Automatic Screen Brightness
> Disable Dim Screen
> Disable Automatic Screen Blank
![Power 4](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-power4.png)
> Once completed, you can exit Settings.


#### 3. Performance Co-Pilot (PCP) 
> 
**SKIP THIS SECTION - RUN AFTER 3rd LAB IF TIME PERMITS**
> 

**Due to overhead - we recommend you skip this section and optionally run it after the 3rd lab**
>



> In this exercise, we will install Performance Co-Pilot (Otherwise known as PCP). This tool will allow for near realtime graphical performance analysis of many metrics - however we will only install just a few of these checks for this workshop.
> PLEASE NOTE:  PCP is great for debugging, capacity planning, and troubleshooting ... BUT ... it does add a significant amount of overhead to any system... Use it accordingly.

> Open a terminal.

```
$  sudo -i

# dnf install -y   pcp  pcp-conf pcp-devel pcp-doc pcp-libs pcp-libs-devel pcp-gui
(output omitted)

# dnf install -y pcp2pdf pcp-pmda-dm pcp-pmda-bash pcp-pmda-lmsensors
(output omitted)

# dnf install -y  pcp-pmda-memcache pcp-pmda-netcheck pcp-pmda-podman pcp-pmda-rsyslog
(output omitted)

# dnf install -y  pcp-pmda-sockets pcp-pmda-summary pcp-pmda-trace pcp-pmda-systemd pcp-system-tools

# reboot

```

> Once the system has rebooted, log back into Gnome Desktop.


> Go to the applications selector (upper left hand corner) and scroll until you find "PCP Charts" - click on the icon.
![PCP 1](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-pcp1.png)



![PCP 2](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-pcp2.png)



![PCP 3](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-pcp3.png)




![PCP 4](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-pcp4.png)




![PCP 5](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-pcp5.png)




![PCP 6](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-pcp6.png)




![PCP 7](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-pcp7.png)










#### 4. TUNA & TuneD optimization

![Enable tuned](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-tuned1.png)

> As root, in a terminal, type "tuna"
> The TUNA interface will appear - confirm the autocorrect by clicking "YES" 
![Initial tuna](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-tuna1.png)


> REBOOT now
> Login, open a terminal and reopen the tuna interface

![tuna screen 1](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-tuna2.png)


![tuna screen 2](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-tuna3.png)


![tuna screen 3](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2a-tuna4.png)




#### 5. System patching
> Before we get into the AI section of this workshop, we'll update the system and reboot.
> Open a terminal and update the system.
> PLEASE NOTE: This will take several minutes. Take a quick break....

```

$  sudo -i

#  dnf update -y 
(output omitted)

```

#### 6. Reboot
> Once all the patching has completed, you need to reboot/restart the system.

```

# reboot

```


> This is the end of this exercise


