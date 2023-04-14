OpenArenaPandora
================

OpenArena version for OpenPandora / ODroid / RPi, featuring ARM support and GLES renderer.

The current state is playable without any major problems and good performances. 
Only limits are len flares that requires depth buffer reading and so are disabled.
Note that this version integrate a QVM with a JIT backend on ARM, so bots doesn't slow down the games too much.

OpenPandora / ODroid / RPi
===========

This version is aimed at OpenPandra, so get:
 * ARM compatibilty (using -DARM)
 * Some NEON optimized code (using -DNEON)
 * GLES renderer (using -DHAVE_GLES)
 * Toggle Crouch function (using -DCROUCH), disabled by default and with a new option in cfg
 * OpenPandora support of course (using `make PANDORA=1`), for screen resolution mainly.
 * ODROID support (build with `make ODROID=1`), mostly like Pandora, but without the control and resolution hack
 * RPI support (build with `make RPI=1`), same as ODROID (will not work for RPI 1, has NEON support is compiled in)
 * RISC-V 64 support (build with `make RV64=1`) will build an OpenGL version without compiled VM

Note that RPI build is untested, any feed back is welcome.

For more info on the OpenPandora go here: http://boards.openpandora.org/
Specific thread for Jedi Academy on the OpenPandora here: http://boards.openpandora.org/index.php/topic/13695-open-arena/
