Some basics for Feebsd set up... work in progress. 
Use desktop-installer for setting up desktops. 
This is mostly a lot os commands that I can't remember so this page saves me an internet search.

Lost virtual consoles after upgrade to 14.2..

Had same issue with amdgpu graphics card and i915kms graphics card.

Do this as root user:--  "cd /usr/ports/graphics/drm-61-kmod" and "make install" worked perfectly for me..
