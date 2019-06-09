# What is the purpose of this repo

This is... lets call it a "continuation".... of the work that the team behind the Pro CFW has worked so hard on in the past. Now that the PSP is well abandoned, I'd like to see if I can revive some of the Sony created features. Things like, the PSN store. I'll be up front, all my coding knowledge is self-taught (and primarily in C#/PHP), so this is a big learning curve for me (I've dabbled very little in c/c++, enough to rebuild NitePR from source when that was still a thing). But, I still want to at least give this a go. Hopefully this actually works out, but even if not, there now exists, a record of my attempts that [maybe] someone with more skill than I can look at in the future.

# What will this be called?
I have no idea. Back when Dark Alex was actively making firmwares, I was a fan of the M33 nomenclature, however that's already happened. There's no need to revive a naming scheme that's attached to someone much more talented than I (plus, I'm not about to ride on his fame by making people think this is his work). In all honesty, it'll either be named something related to my handle (Giga/Gigawiz) or the gaming community that my friends and I run (Pew Pew Kittens). I'll probably revisit this later.

# Can I help?
Sure, if you want. But keep in mind, you're dealing with someone who is the _literal_ definition of "noob" when it comes to developing for the PSP. That being said, you're welcome to pull the code (god help you) and do some changes. If you're interested in discussing the project, I'll be hiding in a new discord that can be found [here](https://discord.gg/PZAeJ5t)

# Planned Features
* Custom, Built-In replacement for the PSN store
  * Download PSP ISO/CSO Games (from the plethora of sites on the web that supply these)
  * Download Homebrew Apps (Either from a hand-coded server that will also be open-sourced, or from the various homebrew-related sites that already exist)
  * Download custom themes/boot animations 
* Theming engine that allows a complete overall redesign of the UI (so the XMB could look more like... say Android or IOS, but without needing to directly edit the code of the firmware itself)
  * Probably going to try to fiddle with the CXMB source, as that seems like a good starting point (Only seen a video on youtube about it, but it seems like this plugin does **exactly** this)
* Continuation of the (Now defunct?) Prometheus/aemu Ad-Hoc Multiplayer Server
* More to come as I complete those planned things....

# Details about the Folder Structure

* SystemControl: kernel of CFW
* Rebootex_bin: patch reboot.bin and redirect the loading of bootconfs
* Rebootex: load rebootex.bin into kernel and boot the whole CFW
* Vshctrl: all VSH related patch goes here. And the ISO VSH dipslay code too.
* ISODrivers: march33 and galalxy included for ISO loading
* Popcorn: for custom PS1 hack
* Installer: install the CFW into the system. After that it can use Rebootex to boot into CFW.
* CIPL: permanently install 635PRO on 01g/02g
* Satellite: VSH menu
* Recovery: Recovery menu as those in 5.XX kernel
* testsuite: test tool/homebrews/utils for 635PRO
* FastRecovery: Boot the 635PRO faster once installed
* include: common used header goes here
* libs: common used library goes here
* contrib: scripts or else goes here
* docs: complex documents goes here
* Common: Common code goes here
* Imports: The imports of 635 functions go here
