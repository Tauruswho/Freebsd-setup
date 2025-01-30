Some basics for Feebsd set up... work in progress.
This is mostly a lot commands and examples that I can't remember so this page saves me an internet search.

I use "desktop-installer" for setting up desktops for first install. 

Lost virtual consoles after upgrade to 14.2..

Had same issue with amdgpu graphics card and i915kms graphics card.

Do this as root user:--  "cd /usr/ports/graphics/drm-61-kmod" and "make install" worked perfectly for me..

# Shutdown not working try this...
hw.efi.poweroff=0 ## in /etc/sysctl.conf

