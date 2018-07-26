Xiamo Mi Notebook Pro
===========
Installation and setup on Linux Mint 18.3

![!](http://i.cubeupload.com/ZIhUa4.png) Disclaimer
------------
This is only some reminders for myself.

Use this tips at your own risk.



Pre-installation
------------
Enter UEFI by pressing the F2 key several times during the boot.

Disable UEFI and secure boot



Mint installation
------------
Install Linux Mint 18.3 with full disk encryption

Enable intel-microcode + nvidia-384 in the Driver Manager

Reboot

Type some shits in terminal :
- sudo add-apt-repository ppa:jd-team/jdownloader
- sudo apt install gparted redshift-gtk jdownloader git samba
- sudo sh -c "echo '\nHISTFILESIZE=20000\nHISTSIZE=20000\nHISTCONTROL=ignoredups' >> /etc/environment"
- sudo bash -c "echo export MOZ_USE_OMTC=1 >> /etc/X11/Xsession.d/90environment"
- sudo ufw enable

Install Waterfox instead of Firefox

By default the FN keys are enabled. 
Press FN + Esc to switch the FN keys functionnality

Turn off bluetooth at startup: 
- sudo nano /etc/bluetooth/main.conf
- Uncomment AutoEnable=false

Fingerprint:
https://github.com/iafilatov/libfprint/issues/2


SSD Speed optimization
------------

Check BIOS version with: sudo dmidecode -t bios -q

Follow the instructions provided here to make the thumb drive: 
https://techtablets.com/2017/12/xiaomi-mi-notebook-pro-nvme-ssd-bios-pcie-x2-fix/

- Press F2 several times during the boot to enter in UEFI
- Enable UEFI
- Press F12 several times during the boot to select the thumb drive
- Type unlockme
- Press F12 several times during the boot to select the thumb drive
- Type flash
- Pray
- Press F2 several times during the boot to enter in UEFI
- Disable UEFI


Sources
------------
https://askubuntu.com/questions/67758/how-can-i-deactivate-bluetooth-on-system-startup

http://bbs.xiaomi.cn/t-13986845

https://www.youtube.com/watch?v=q0k6Uv3dtEE


Contact
------------
You can contact me at: string.Format("{0}#{1}","its.skway","gmail.com").Replace("#","@");


Donations are welcome:
- BTC: 174Eud8voesGp3YcpzjZJGjcjYAr2V42fH

Written by Skw4y in 2018. Released under the terms of the MIT License.
