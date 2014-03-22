Skeinforge50plus
================

Skeinforge50 (the last release from Enrique) with a few tweaks:

* Bug fixes

* DeuxVis and Joost-b improvements to Cool with regard to fan control (see http://forums.reprap.org/read.php?154,149615,245895)
  - turn on fan at beginning
  - do not use fan before layer N
  - set fan maximum speed
  - force fan on bridging layers (requires enabling Inset -> Infill in direction of bridge)
  - maximum layer time time for fan 
  - turn on fan at full speed on layers less than N sec 


* Theodleif improvement to skirt plugin to add a "brim" (see http://forums.reprap.org/read.php?1,136147,136147#msg-136147)
  - brim width in number of loops


* Dimension plugin improvements
  - firmware retraction via G10/G11 (e.g. supported by Marlin). If set the retraction speed, distance, and extra restart distance are ignored

