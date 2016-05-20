OpenArenaPandora
================

OpenArena version for OpenPandora, featuring ARM support and GLES renderer.

The current state is playable without any major problems and good performances. 
Only limits are flares that requires depth buffer reading, and QVM that is interpreted (no JIT on ARM)

OpenPandora
===========

This version is aimed at OpenPandra, so get:
 * ARM compatibilty (using -DARM)
 * Some NEON optimized code (using -DNEON)
 * GLES renderer (using -DHAVE_GLES)
 * Toggle Crouch function (using -DCROUCH), disabled by default and with a new option in cfg
 * OpenPandora support of course (using -DPANDORA), for screen resolution mainly.
 * ODROID support (build with make ODROID=1), mostly like Pandora, but without the control and resolution hack

There are some hard-coded value in the Makefile, located at the beggining to force "OpenPandora version" (COMPILE_PLATFORM=pandora and COMPILE_ARCH=arm).
 
For more info on the OpenPandora go here: http://boards.openpandora.org/
Specific thread for Jedi Academy on the OpenPandora here: http://boards.openpandora.org/index.php/topic/13695-open-arena/
