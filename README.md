Skeinforge50plus
================
[Poikilos Fork](https://github.com/poikilos/Skeinforge50plus)

## Reasons for fork:
- Preserve this great program, which adds to the public-licensed 3D
  printing ecosystem.
- Make better documentation (Recover usable
  website & wiki information from web.archive.org and bmander's
  README.markdown) and user self-support path such as a forum.
  - See also [Skeinforge](https://reprap.org/forum/list.php?154) on
    RepRap Forum.
- Make a fancy modern UI.
- Choose a better name.
- Add fancy supports.

## Why Skeinforge is still good
- Skeinforge performs better than Cura in some
  cases. A test print and the claim that Cura is based on an "old fork"
  of Skeinforge is at:
  http://reprap-art.blogspot.com/2019/01/whats-better-skeinforge-or-cura-engine.html
  - He uses "Slow Down" for "Cool Type" to avoid wavy layers on narrow
    pillars and a pointy artifact on the top of the [Calibration
    Temple](https://www.thingiverse.com/thing:1019953) (he actually
    mentions thing:10199530 which no longer exists, but the new
    BrunoBellamy Sep 17, 2015 upload is apparently the same).

## Why Skeinforge went away
- A big reason for the program's demise may be that the website's hard
  drive crashed and the Wiki was never recovered (and the website had a
  huge span of downtime).
  - I will see what I can recover from the wayback machine.

## Tasks
- [ ] Consider PyPy for JIT compiling.
- [x] Add later tweaks--consider forking from indazoo's fork:
  [nophead/Skeinforge50plus](https://github.com/nophead/Skeinforge50plus)
  "Skeinforge50 (the last release from Enrique) with a few tweaks"
  - Use indazoo's more recent version with more changes:
    https://github.com/indazoo/Skeinforge50plus
    (forked from AlexeyKruglov's, which also has several changes)
- [ ] Ensure good plugins are included, such as "stretch" (arc
  compensation) by Enrique Perez:
  https://blog.pcedev.com/2015/06/02/arc-compensation-reprap/
- [x] Ensure github.com/ahmetcemturan has commits for all versions
  (compare to
  http://web.archive.org/web/20160606125233/http://fabmetheus.crsndoo.com/index.php?all=true)
  - Times are in CET timezone (Central European Time (CET) UTC+01:00)
  - or from http://web.archive.org/web/20110401000000*/http://members.axion.net/~enrique/reprap_python_beanshell.zip
    "the unstable skeinforge is on my website at [http://members.axion.net/~enrique/reprap_python_beanshell.zip](http://members.axion.net/~enrique/reprap_python_beanshell.zip)" (http://fabmetheus.blogspot.com/search?updated-max=2010-10-24T03:21:00-07:00&max-results=7)
- [ ] Compare to
  https://github.com/ahmetcemturan/SkeinForgeGIT/commits/master
  (some recent commits differ).
  - [x] just IntelliJ IDEA metadata (.idea directory)
  - [ ] Improved .gitignore and other changes: https://github.com/ahmetcemturan/SkeinForgeGIT/commit/b1be44ee60c78c00f04b7241159fd91611805c76
- [ ] Revise and re-add parts of bmander's README as necessary:
  https://github.com/bmander/skeinforge/blob/master/README.markdown
- [x] (SOLVED: bmander had outdated copy--fork from ahmetcemturan
  instead.) Add license -- The original README.markdown says "GPL" but
  other sources say it is GNU Affero General Public License
  http://www.gnu.org/licenses/agpl.html:
  - https://github.com/nophead/Skeinforge50plus/blob/master/skeinforge_application/skeinforge.py
  - https://github.com/garyhodgson/SkeinforgeEngine
    - http://garyhodgson.github.io/SkeinforgeEngine/apidocs/plugins.comb-module.html
  - http://buildatron.com/facts-sfact
- [ ] Implement Veroni supports
  - [x] wait until a license gets added to voronizer (I
    [requested](https://github.com/tjwill95/voronizer/issues/1) that).
- [ ] Implement automatic model turning for least support using
  turnit if license gets added (I
  [requested](https://github.com/nickc92/turnit/issues/1) that.)
- [ ] Make temperature tower feature: Allow user to merely enter the max
  and min temperature for the filament).
- [ ] Pick a different name (see "Possible Alternate Names" below)

## History of Skeinforge Author's Website
- The original author is Enrique Perez according to
  https://books.google.com/books?id=cnH1SGiv2BcC&lpg=PA283&ots=RBpiwZtiu8&dq=what%20happened%20to%20enrique%20skeinforge&pg=PA283#v=onepage&q&f=false
  - See his posts at https://reprap.org/forum/search.php?154,author=488,match_type=USER_ID,match_dates=0,match_threads=0
    - The last post is https://reprap.org/forum/read.php?233,108249,108542#msg-108542
      December 01, 2011 07:39PM
  - His last Skeinforge commit is Apr 27, 2011 at
    https://github.com/amsler/skeinforge/commits/master
    - It is Skeinforge 41, but I have later versions from
      web.archive.org.
- Complete site last seen before ad site:
  - http://web.archive.org/web/20160401000000*/http://fabmetheus.crsndoo.com/
  - ...
  - http://web.archive.org/web/20160805002741/http://fabmetheus.crsndoo.com/
- Downtime showing ad site:
  - http://web.archive.org/web/20160830122431/http://fabmetheus.crsndoo.com/
  - ...
  - http://web.archive.org/web/20161123102129/http://fabmetheus.crsndoo.com/
  - http://web.archive.org/web/20160830122431/http://fabmetheus.crsndoo.com/
  - ...
  - http://web.archive.org/web/20170428041951/http://fabmetheus.crsndoo.com/
- Says "In March 2017 we had HHD crash." Links to zips are NOT
  archived by wayback machine from this time onward:
  http://web.archive.org/web/20170527034851/http://fabmetheus.crsndoo.com/
- Other releases not archived on http://web.archive.org/web/20160606125233/http://fabmetheus.crsndoo.com/index.php?all=true
  - [2010-01-15 21_57_57](http://web.archive.org/web/20141211202524/http://fabmetheus.crsndoo.com/files/9_reprap_python_beanshell.zip)

## Developer Notes
### Possible Alternate Names
- SFR Slicer (Skein Reborn Slicer)

### indazoo's notes
Skeinforge50 (the last release from Enrique) with a few tweaks:

* Bug fixes

* DeuxVis and Joost-b improvements to Cool with regard to fan control (see http://forums.reprap.org/read.php?154,149615,245895)
  - turn on fan at beginning
  - do not use fan before layer N
  - set fan maximum speed
  - force fan on bridging layers (requires enabling Inset -> Infill in direction of bridge)
  - maximum layer time time for fan
  - turn on fan at full speed on layers less than N sec
  - when using slow-down, set minimum feed rate

* Theodleif improvement to Skirt plugin to add a "brim" (see http://forums.reprap.org/read.php?1,136147,136147#msg-136147)
  - brim width in number of loops

* Dimension plugin improvements
  - firmware retraction via G10/G11 (e.g. supported by Marlin). If set the retraction speed, distance, and extra restart distance are ignored

* delsydsoftware improvements to Fill plugin (see http://www.thingiverse.com/thing:65624)
  - The ability to disable the top layers of a model for printing out cups, vases, or other hollow objects without deleting lines from gcode manually
  - An automatic solid surface thickness feature, which lets you set the thickness of top, bottom, and overhang surfaces in milimeters, instead of layers. This keeps top and bottom surfaces proportional, even when printing in thin layer heights. It results in much cleaner top and bottom surfaces, even with ridiculously low infill settings and small layer heights.
  - Forcing even/odd top layers. The fill patterns on the top layer of a surface are different, depending on whether there are an even or odd number of solid surface layers. I prefer to see the even layers, which use vertical lines. Odd layers tend to use slanted lines, which print more slowly and can be a bit messier. You can now choose whether you want the final layer to be even or odd.
 - You can now determine how much of the object to print using the 'Object printing percentage/layer limit' feature. This lets you print 1 layer of an object, which can be handy for printer calibration. It also lets you print a custom percentage of the object, or a custom number of layers. This feature is disabled by default, and is ignored if you have Disable Top Layers enabled.

* svanteg improvement to Raft plugin for first layer support (see http://forums.reprap.org/read.php?154,350315,350315#msg-350315)
  - support flow rate over operating rate (first layer)
