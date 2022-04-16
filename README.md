# CAPshift3.0 (Continuation and evolution of CAPshift and CAPshift 2.0)

![CAPshift3](https://user-images.githubusercontent.com/1145722/163673868-b3ae0222-9378-49b9-aa80-ed22e74f540a.png)

## CAPshift is a Caps Lock (and optionally NumLock and Insert Lock) extender!

CAPshift creates a minuscule (customizable delay so that the capslock key can't just be knocked by mistake whilst typing, and must be held for x milliseconds to activate.
Also if capslock is held for a longer period of time, it displays a menu that extends the caps lock key. Offering functions such as: convert selected text to UPPER CASE, lower case, Title Case, Sentence case, or iNVERT cASE.

After discovering the original CAPshift by skrommel and modifying it for my own use over 3 years ago now, I've always intended to add the same functionality to the numlock key, as I often toggle numlock accidentally, and as a laptop user it can be a real pain.
I thought I'd take the opportunity to incorporate all the cool functionality everyone's added to CAPshift over the years, and make the extra features optional so people don't have to 'pick a version' depending on what features they do or don't want. So have made a CAPshift 2.0 that tries to incorporate everyone's additions and improvements.

CAPshift3.0 (and 2.0) is based off of K.Freeman's version of the script as it included INI configuration support, allowing the user to toggle which features they want to use, as well as most of the features of each contributing author.
https://autohotkey.com/board/topic/4310-capshift-slow-down-and-extend-the-caps-lock-key/#entry360797

I got fed up with activating overtype all the time and typing over all my text. Finally decided to add support to CAPshift which I've been happily using now for 8 years. Also, it includes a couple of menu items I added over the years to make copy pasting text into windows filenames a lot easier.

Main new features of CAPshift 3.0:
* Support for Insert Lock. Note insertlock/overtype mode is per app, rather than global like numlock/capslock.
* Menu option to strip characters forbidden in Windows filenames.

Main new features of CAPshift 2.0:
* Optional functionality saved to INI file. So everyone can pick and choose their preferred features from each version of the scripts, such as: progress bar visibility, color, tooltips, capslock toggle menu item or split on-off menu items in enhanced menu.
* Added delay and menu functionality to NumLock and capslock.
* Fixed K Freeman's script (but bug has existed since skrommel's original script) so that hitting a modifier key (such as shift which is right below capslock) at the same time as capslock doesn't bypass the script.
* Put capslock ON and Capslock OFF back in menu (and NumLock ON and OFF). INI option to switch back to toggle menu items instead.
* Fixed K.Freeman's bug which prompts for a custom timer of 1 second=1000 but timer loop uses a sleep 10 in the loop making 1 second=100. Updated prompts to reflect the meaning of numbers.
* Reorganised the menu. As features are added it makes more sense to cascade the text conversions

I've also incorporated HansBKK's request and Gogo's "Needle" code into CAPshift to add a Smart Title Case function in addition to the dumber Title Case function, it seemed like a cool idea, so I fiddled around trying to add it to CAPshift2. Basically it does not capitalize articles, conjunctions, and prepositions unless they are in the start of the sentence. Gogo's sample list of these words were very limited, so I extended it.

Finally, I've added a feature to make the capslock (and numlock if numlock mode is enabled) immediately induce the menu rather than toggle capslock at all, based on HansBKK's use case. I didn't actually use any of his code but give credit for the idea.

New features and script author they came from:
evl:
* Color progress bar (I have modified this to allow custom colors)
* remove under scores
* remove fullstops
https://autohotkey.com/board/topic/4310-capshift-slow-down-and-extend-the-caps-lock-key/#entry145316


k freeman:
* Sentence Case function (removed yes/no dialog if you don't want lowercase proper nouns don't use the feature or go back and capitalise the proper nouns manually).
* ini settings support
https://autohotkey.com/board/topic/4310-capshift-slow-down-and-extend-the-caps-lock-key/#entry360797

GoGo:
* Smart Title Case
https://autohotkey.com/board/topic/72876-why-isnt-this-uppercase-script-working/#entry462990
Credit to HansBKK for the suggestion.

# Autohotkey
This is an AutoHotkey Script. To create an executable from it download AutoHotkey from autohotkey.com and use AHK2EXE to compile it into IdleLock.exe
