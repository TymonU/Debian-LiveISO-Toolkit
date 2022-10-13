# Debian-Live-Script
Small script to make a live iso from debian based installs. 

Be sure to install all the depends. 

Depends: Install command

apt install rsync live-boot systemd-sysv debootstrap squashfs-tools xorriso isolinux syslinux-efi grub-pc-bin grub-efi-amd64-bin grub-efi-ia32-bin mtools dosfstools resolvconf

Be sure the installed kernel supports aufs

Inside the makelive script there are three variables. Change their values to your preference using a text editor.

Be sure the script is executable and you are either logged in as root or you are on the terminal under su

chmod +x makelive

su password


To use it just ./makelive

Give it time and it will make a live bootable iso of your current install directly into your home folder.

Enjoy!

P.S. It does not care what DE you are using. 
