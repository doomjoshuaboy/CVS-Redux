Capcom VS SNK REDUX IKEMEN Screenpack

This is an nightly only Screenpack. So if you put it in older IKEMEN and MUGEN or WinMUGEN, IT WILL NOT WORK!!!

Welcome to This Customised Screenpack all by DoomJoshuaBoy.  

This is inspired by CAPCOM VS SNK 2 game, all rights reserved.

Also please considering having at least 3-4 gb of ram as this screenpack is heavy resources

Supporters:

2Dee4ever
ArachnoLord
Hollow
ViolinKen
RagingRowen
Bluekuma
POTS
Akito (Huge Helper)
ShinZankuro

Original authors:

Raisu
PabloSSB
ProtomanX
-Shin_Hado-

Thanks to:
POTS (for Capcom VS SNK 2 commentator system, Attack data and active tag modules)
Kamekaze (for Round Transition Module)
 


Since this Screenpack includes some ZSS or Lua that needs replacement, this section is required:
To Add EXTRAS:  
Load IKEMEN_GO first then close it OR Exit, it will give you extras in your "save" Folder,
Open up the folder you should see a "config.ini" File load it up with your favorite Text editor (Recommendation: Visual Studio Code or Notepad++)

`[Common]
; Common animations using character's local sprites
Air     = data/common.air
; Common commands
Cmd     = data/common.cmd
; Common constant variables
Const   = data/cvsr/fight/cvscommon.const
; Common states (CNS or ZSS)
States  = data/functions.zss, data/cvsr/fight/ZSS/cvsaction.zss, data/cvsr/fight/ZSS/cvsdizzy.zss, data/cvsr/fight/ZSS/cvsguardbreak.zss, data/score.zss, data/system.zss, data/cvsr/fight/ZSS/cvsactivetag.zss, data/training.zss
; Common packs of graphic and/or sound effects called during the match by using
; a specific prefix before animation and sound numbers (like lifebar fightfx)
Fx      = data/cvsr/cvsfx.def, data/cvsr/fight/commentator_cvs2.def, data\CVSR\fight\cvs_roundtransition.def
; External modules (no need to add modules placed in external/mods directory)
Modules = data/cvsr/lua/fadesnd.lua
; Pure Lua code executed on each frame during match
Lua     = loop()
; Common states (CNS or ZSS)
States0 = data/cvsr/fight/ZSS/cvsko.zss, data/cvsr/fight/ZSS/cvsrounds.zss, data/cvsr/fight/ZSS/roundtransition.zss, data/cvsr/fight/ZSS/intro-outro.zss, data/cvsr/fight/ZSS/intro-outro-config.zss, data/cvsr/fight/ZSS/cvsconfig.zss, data/cvsr/fight/ZSS/commentator_cvs2.zss, data/cvsr/fight/zss/attackdata.zss
`

Then go down and change "GameWidth" and "GameHeight" to however you want, then
change "Motif" to either
There's 2 seprated motifs

HD
Squared:
[Config]
; Motif to use. Motifs are themes that define the look and feel of Ikemen GO.
Motif               = data/cvsr/systems.def

Diamonds:
[Config]
; Motif to use. Motifs are themes that define the look and feel of Ikemen GO.
Motif               = data/cvsr/system.def
