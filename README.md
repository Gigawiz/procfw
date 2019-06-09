# What is the purpose of this repo

This is... lets call it a "continuation".... of the work that the team behind the Pro CFW has worked so hard on in the past. Now that the PSP is well abandoned, I'd like to see if I can revive some of the Sony created features. Things like, the PSN store. I'll be up front, all my coding knowledge is self-taught (and primarily in C#/PHP), so this is a big learning curve for me (I've dabbled very little in c/c++, enough to rebuild NitePR from source when that was still a thing). But, I still want to at least give this a go. Hopefully this actually works out, but even if not, there now exists, a record of my attempts that [maybe] someone with more skill than I can look at in the future.

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
