                          ______________________________________________
=========================| Attack Data Display by Phantom.of.the.Server |==========================
                          ¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯        [01.02.2025]

 - Contact: potsmugen@gmail.com
 - Website: https://network.mugenguild.com/pots/
 - If you downloaded this file from anywhere else, it's probably outdated
 
 - Training mode attack data display system for Ikemen GO January 2025 build and above
 - For older versions for older engines, try searching my Mediafire folder



=========================================< INTRODUCTION >==========================================

This system adds some attack data display to Ikemen GO's native training mode.

The aim was to make something simple to use and to install that still gives you the information you need.

It displays the following information:

Hit Damage ---- Damage dealt by the last hit
Combo Damage -- Damage dealt by the last combo
Max Damage ---- Highest combo damage so far
Max Combo ----- Longest combo so far
Advantage ----- Frame advantage of the player character before both characters returned to idle
Startup ------- How many frames the last attack took to hit the training dummy

If the Startup of an attack is less or equal than the Advantage of another attack, then those two attacks can be linked.

If practicing in Tag mode, Advantage and Startup will refer to the point character.
In Simul mode, they will refer to the player closest to the dummy.

The text display can be hidden by pressing start with the dummy's controller.



=========================================< INSTALLATION >==========================================

 - Move the contents of the archive into Ikemen GO's "data" folder

 - Inside Ikemen's "save" folder, open the "config.ini" file with a text editor

 - In the "[Common]" section, find or make a new "States" line and add "data/attackdata.zss" to it. Example:

    [Common]
    States1 = data/attackdata.zss

 - You're all set



============================================< F.A.Q. >=============================================

Q: I don't like how the text looks. Are there any configuration options?
|
A: Open the "attackdata.zss" file, check the "Configuration" section at the top of the file and change the values to your liking.



Q: All that text gets in the way sometimes. Can it be turned off?
|
A: Yes. Press start with Player 2 (training dummy).



Q: I noticed this module slows down Ikemen. What can I do?
|
A: Ikemen GO's text display is unoptimized, so on some hardware it may impact performance.
Try switching to a font that uses a SFF instead of TrueType.



Q: I manually counted the frames and found an attack that is -3 while your data says it's -4. What's up with that?
|
A: The vast majority of characters cannot attack in the frame where they return to an idle state. So I opted to not count that frame towards frame advantage.

Note 1: Contrary to Mugen, in Ikemen 0.99 characters can guard in that first idle frame.
Note 2: Characters using my old "tick fix" code can indeed attack in that frame, but they are a very small minority and there is no way to detect if that code was used anyway.



If your question isn't answered here, or for general feedback, drop me an email if you want.



=========================================< KNOWN ISSUES >==========================================

 - Startup calculation is a bit rough due to it being impossible to predict in every situation. I think it gets the job done, however
 - Zero or healing "damage" will not be displayed correctly. I might revisit this if it's proven to be a useful feature



=======================================< VERSION HISTORY >=========================================

<01.02.2025>
 - Added some config options
 - Added guard level display

<25.02.2024>
 - Fixed frame advantage while players are paused
 - Positive advantage now shows a plus sign
 - Frame advantage value is now optionally color coded
 - Refactored the code so that chip damage without gaps also shows as combo damage

<03.02.2024>
 - First release



========================================< WHAT'S MISSING >=========================================

 - Nothing at the moment



========================================< SPECIAL THANKS >=========================================

 - wily-coyote, for adding the guard level trigger to Ikemen GO
 - The Mugen Fighter's Guild Discord. I made this because people sometimes asked where to get one
