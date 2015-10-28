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

Further information on the LKE Unicode version
----------------------------------------------

Carthage Sans LKE is an expanded Unicode version. It aims to cover as much as possible of the Latin, Cyrillic, and Greek blocks of the Unicode standard (thus the initials -- "Latina, Kirilitsa, Elleniki"). I'm open to expanding it to any of the other scripts Unicode covers, but I have little to no personal experience with most other alphabets; if you'd like to contribute, I'd particularly be interested in Arabic, Devanagari, Katakana, Hiragana, Armenian, and Hangul. (I would like to add Hebrew as well, but it's hard to get the diacritics right in what's essentially a pixel font. We'll see.)

The current status as of 10/28/2015 (the date of initial publication): 

-Latin: all of Latin-1, Latin Extended-A, and "Even More Latin"; Latin Extended-B is missing some characters that seem to be mostly either phonetic notation or obsolete.
-Greek: All Greek characters supported by FontStruct; if you need letters like heta or Pamphylian digamma, those will probably be added to the GitHub version. FontStruct does not provide polytonic Greek support, so that too will be added later. Coptic letters are not supported; I don't see a lot of need for them but they won't be a problem to add on request.
-Cyrillic: Still a work in progress, but all Slavic languages using Cyrillic characters should be covered. The main holdup is Abkhazian, which is spoken by just over 110,000 people in the world and also has one of the longest alphabets in the world; I have no idea how many of them would be interested in this, so it hasn't been a huge priority. (Besides, the PT family from Russia's Paratype is excellent and far better than I could do with most Cyrillized languages.) 

I've emphasized support for several languages, the most important being Vietnamese (75 million speakers deserve some support no matter how tedious it is to do so). I've also added characters for Old Irish, Old Church Slavonic, and Icelandic. There's a number of characters used in pan-African linguistics I am not sure if I need or not; they'll get filled in eventually alongside the Cyrillic, but how fast I have no idea. 

Major change log
----------------

20151028: Finally enough of the LKE version is finished to upload to GitHub
20151026: Learned some new techniques in Fontstruct, and thereby cleared up some annoying font geometry issues (most notably the pixel-accurate but hideous upper case W). 
