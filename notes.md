This document contains various random bits of information that may be of some interest to the user and/or hacker.

* FontStruct generates slightly wonky TrueType code for some characters, so if you generate a font from its SFD file, FontForge is liable to complain about it. It should work fine if you just ignore the errors, but let me know if you find otherwise.
* I'm not particularly happy with the very heavy weight of the bold version; it's mostly that way to match up with the original bitmap, and I don't like it. Expect a demibold at some point. (Also, don't expect ligatures in the bold face. They'd just wind up looking like blobs.)
* The line segments making up the outlines will be very obvious at large point sizes. This will require extensive tweaking in FontForge and I'm just not sure I care all that much.
* For German speakers: The choice of a Fraktur-inspired shape for the upper case Eszett glyph is entirely arbitrary and somewhat rooted in the fact that there wasn't an obvious way to distinguish it from a lower-case Eszett or a capital B. If this is a problem, let me know and I'll see what I can do.
