Some basics for Feebsd set up... work in progress.
This is mostly a lot commands and examples that I can't remember so this page saves me an internet search.
I had a few issue on the way, not all directly Freebsd related, see below:-

I use "desktop-installer" for setting up desktops for first install. But many guides on line to follow:-

https://www.server-world.info/en/note?os=FreeBSD_14&p=download

Lost virtual consoles after upgrade to 14.2..

Had same issue with amdgpu graphics card and i915kms graphics card no virtual consoles.

Do this as root user:--  "cd /usr/ports/graphics/drm-61-kmod" and "make install" worked perfectly for me..

Shutdown not working try this...
hw.efi.poweroff=0 ## in /etc/sysctl.conf

My ASUS maxium V extreme motherboard had the wrong MAC address "88:88:88:88:87:88". Booted into usb stick with Linux Mint and followed this guide:-

https://askubuntu.com/questions/1338578/mac-address-stuck-at-888888888788

Using eeupdate64e for linux... It worked...

Modify your bios for nvme boot:----  
https://winraid.level1techs.com/t/howto-get-full-nvme-support-for-all-systems-with-an-ami-uefi-bios/30901

Had loads of problems with WD SN580 1TB and SN770 1TB NVME M.2 drives stopping or faulting causing degraded zpools. Needed to update firmware follow guide below:-
Tried windows WD update (WD-Dashboard) utils but they did not work for me!!!!!

https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616

See copywholesystemtonew-disk if you need to clone a good installed system...
