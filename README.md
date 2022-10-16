# Debian-LiveISO-Toolkit
Currently a small script to make a live ISO from debian based installs. This is NOT a fork of other liveISO creators. Remastersys was the best of the lot of them and it is no longer working. The forks are no longer supported. Systembak is broken. I have never been able to get Linux-Live to work.

Be sure to install all the depends. 

Depends: Install command

apt install rsync live-boot systemd-sysv debootstrap squashfs-tools xorriso isolinux syslinux-efi grub-pc-bin grub-efi-amd64-bin grub-efi-ia32-bin mtools dosfstools resolvconf gparted

Be sure the installed kernel supports aufs

Inside the makelive script there are four variables. Change their values to your preference using a text editor.

Make the script executable, log in terminal as super user and execute. It will take time.

chmod +x makelive

su password

./makelive

Give it time and the ISO will be in a /home folder of the USERNAME defined in the makelive script file. debian-user by default.

Enjoy!

Upcoming features:
- Optional creation of a live user that has sudo privilages and no password
- Optional enabling of Plymouth Splash Boot Screen
- Option to enable persistance
- Installer to install live running OS created by script.
- Optional GUI to make it all point and click
- Deb package and icon to make it installable and runable as command or from menu
