# Optimizing Fedora
A hands-on workshop

[BACK to HOMEPAGE](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/README.md)



## Overview
Now, we will install addtional packages, optimize the desktop and tune the systems in preparation for the setup of our AI environments.

## DEMO One: 
Matt will demo the multiple steps to enhance, tune and optimize the Fedora 42 environment in preparation for the AI installations.
![DC Roma II Laptop](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab1-start.jpg)

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

#### 3. Configure Date/Time
> Open the Settings menu

> Scroll down and Select: System
![System Menu](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-daytime1.png)

> Select: Date & Time
![Date Time Options](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-daytime2.png)

> Activate: Automatic Time Zone & Clock & Calendar: Weekday by clicking on the activation switch.
![Enable Date Time options](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-daytime3.png)

> exit Settings

#### 4. Disable Bluetooth
> Disabling Bluetooth as it's not needed - and anything not needed should be disabled for security reasons.
> Click on the upper right hand corner to engage the settings panel.
![See BT](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-BT1.png)

> Click on the "Bluetooth" button (this is a switch that can enable/disable - we don't need to open the full settings dialog)
![BT off](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/images/lab2-BT2.png)

#### x. Custom workshop repository configuration
> information will be provided


#### x. Initial package installation
> Open a terminal session
``` 
$  sudo -i
(enter roma password when prompted)

#  dnf install -y gnome-tweaks 
(output omitted)


#  dnf install -y info 

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

#### x. Online resizing of the root volume


## DEMO Two:
Matt will walkthorough advanced gnome desktop settings/optimization


## Hands-on Exercise Two:
In this exercise we will optimize the desktop configruation.

### STEPS:

#### 1. Gnome Desktop advanced configuration


#### 2. Exit the desktop to allow settings to take effect


#### 3. Log back into the desktop environment
> This is the end of this exercise


## DEMO Three:
Matt will walkthrough how to optimize the system in preparation for the AI applications installation.

## Hands-on Exercise Three:

### STEPS: 

#### 1. Systems settings deep dive


#### 2. Power Management


#### 3. Performance Co-Pilot (PCP) 


#### 4. TUNA & TuneD optimization


#### 5. System patching


#### 6. Reboot
> This is the end of this exercise


