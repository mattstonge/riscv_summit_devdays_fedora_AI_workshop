# Supporting Materials
Additional Useful Information

[BACK to HOMEPAGE](https://github.com/mattstonge/riscv_summit_devdays_fedora_AI_workshop/blob/main/README.md)



## Reference Materials


## Reference Materials


## Running Performance Co-Pilot (PCP) Exercise

### Steps:


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








