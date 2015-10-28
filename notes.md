Development notes
=================

This document contains various random bits of information that may be of some interest to the user and/or hacker.

* FontStruct generates slightly wonky TrueType code for some characters, so if you generate a font from its SFD file, FontForge is liable to complain about it. It should work fine if you just ignore the errors, but let me know if you find otherwise.
* I'm not particularly happy with the very heavy weight of the bold version; it's mostly that way to match up with the original bitmap, and I don't like it. Expect a demibold at some point. (Also, don't expect ligatures in the bold face. They'd just wind up looking like blobs.)
* The line segments making up the outlines will be very obvious at large point sizes. This will require extensive tweaking in FontForge and I'm just not sure I care all that much.
* For German speakers: The choice of a Fraktur-inspired shape for the upper case Eszett glyph is entirely arbitrary and somewhat rooted in the fact that there wasn't an obvious way to distinguish it from a lower-case Eszett or a capital B. If this is a problem, let me know and I'll see what I can do.
* For Cyrillic users: I do not wish to get involved in the Russian vs Serbian italics issue. I therefore do not plan on making a full italic version of Carthage Sans LKE (or Carthage Serif, should I get around to it); you'll get the oblique version, and you will like it. Please write all complaints in either Serbian or Russian, as I can read neither and it will make it easier for me to ignore them.
* I haven't yet decided whether to make UFO files available alongside the SFDs. Since FontForge is a FOSS tool that supports UFO export, I'm not of the opinion that UFOs are really necessary, but the issue mostly comes down to just how fat I want the archive to be. 
* OpenType? Maybe.

Major change log
----------------

20151026: Learned some new techniques in Fontstruct, and thereby cleared up some annoying font geometry issues (most notably the pixel-accurate but hideous upper case W). 
