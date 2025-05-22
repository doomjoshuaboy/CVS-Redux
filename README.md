# Capcom VS SNK REDUX IKEMEN Screenpack

Welcome to This Customised Screenpack all by DoomJoshuaBoy.  

This is inspired by CAPCOM VS SNK 2 game, all rights reserved.

**Also please considering having at least 3-4 gb of ram as this screenpack is heavy resources**

## Supporters

2Dee4ever

ArachnoLord

Hollow

ViolinKen

RagingRowen

Bluekuma

POTS

Akito (Huge Helper)

ShinZankuro

## Original authors

Raisu

PabloSSB

ProtomanX

-Shin_Hado-

## Thanks to
POTS (for Capcom VS SNK 2 commentator system, Attack data and active tag modules)

Kamekaze (for Round Transition Module)


## Instructions
### Since this Screenpack includes some ZSS or Lua that needs replacement, this section is required.
1. Download the [Nightly](https://github.com/ikemen-engine/Ikemen-GO/releases/tag/nightly) And [The Screenpack](https://github.com/doomjoshuaboy/CVS-Redux/releases)
2. Extract Nightly to any folder you want then extract the ScreenPack inside `ikemen_go/data`.
3. Load IKEMEN_GO first then close it OR Exit, it will give you extras in your "save" Folder.
4. Open up the folder you should see a "config.ini" File.
5. Load it up with your favorite Text editor (Recommendation: Visual Studio Code or Notepad++) and replace the first lines.
``` [Common]
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
States0 = data/cvsr/fight/ZSS/cvsko.zss, data/cvsr/fight/ZSS/cvsrounds.zss, data/cvsr/fight/ZSS/roundtransition.zss, data/cvsr/fight/ZSS/cvsconfig.zss, data/cvsr/fight/ZSS/commentator_cvs2.zss, data/cvsr/fight/zss/attackdata.zss
```

7. Go down and change "GameWidth" and "GameHeight" to however you want, 

8. Change "Motif" to either

There's 2 seprated motifs

HD
Squared:
``` [Config]
; Motif to use. Motifs are themes that define the look and feel of Ikemen GO.
Motif               = data/cvsr/systems.def
```
Diamonds:
``` [Config]
; Motif to use. Motifs are themes that define the look and feel of Ikemen GO.
Motif               = data/cvsr/system.def
```

9. Lastly load up ikemengo and it should be good to go.