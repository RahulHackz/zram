# Zram
This is a simple script to enable ZRAM on a Raspberry Pi or on any other Linux system.

This script can AUTOMATICALLY detects the number of CPU cores to allocate to ZRAM computation, disables existing swap and enables ZRAM swap.

Steps to use:
• Download the script and copy to /usr/bin/ folder
> sudo wget -O /usr/bin/zram.sh https://raw.githubusercontent.com/RahulHackz/zram/master/zram.sh

• make file executable
> sudo chmod +x /usr/bin/zram.sh

• edit /etc/rc.local file to run script on boot
> sudo nano /etc/rc.local

• add line before exit 0
> /usr/bin/zram.sh &
