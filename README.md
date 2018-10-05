# Poly-Universe-Sample-Mod
A working example for modding content in Poly Universe. 


This is a simple demo of how to mod content in Poly Universe. It gives you a working example of how to mod the game's music, audio, and localization.

Copy this 'Sample Mod' directory into your local mods directory, then enable it in-game to see it in action.

credits:Music loop from DRFX - https://freesound.org/people/DRFX/sounds/338986/

legal:This mod uses free content from around the internet. Individual assets belong to their respective creators.

**************************************

To replace the game's music, place any of the following files in your mod directory:

Music_Space.wav
Music_Combat.wav
Music_Spring.wav
Music_Summer.wav
Music_Fall.wav
Music_Winter.wav

(Capitalization matters! Make sure your wav files have names like "Music_Spring.wav", not "music_spring.wav")

**************************************

To replace sound effects, place any of the following files in your mod directory:

Button Click.wav
Button Click Back.wav
Button New Game.wav
Dismiss Panel.wav
Open Panel.wav
Transition To Space.wav
Transition To Planet.wav
Menu Pause Enter.wav
Menu Pause Exit.wav
Notification Appear.wav
Colonist Death.wav
Construction.wav
Construction Complete.wav
Explosion.wav
Arrow Impact.wav
Arrow Shooting.wav
Rock Harvested.wav
Rock Harvesting.wav
Ship Landing.wav
Ship Take Off.wav
Sword Impact.wav
Sword Swing.wav
Tree Harvesting.wav
Tree Harvested.wav
Troll Death.wav
Water Splash.wav
Ship Reentry.wav
Ship Crash.wav
Tree Falling Start.wav
Tree Falling End.wav

***************************************

Localization can be added using the Localization.xml file. Each line of text in the game is represented in Localization.xml by
a tag, like so:

<string key='NEW_GAME'> ... </string>

The tag above is used by the 'New Game' button on the main screen. We can define how to say 'New Game' in different languages by
adding them inside this tag, like so:

<string key='NEW_GAME'>
    <en>New Game</en>
    <fr>Nouveau jeu</fr>
    <it>Nuovo gioco</it>
    <de>Neues Spiel</de>
    <es>Nuevo juego</es>
    <pt>Novo jogo</pt>
    <ru>????? ????</ru>
    <sv>Nytt spel</sv>
    <nl>Nieuw spel</nl>
</string>

  The languagues above are English, French, Italian, German, Spanish, Portuguese, Russian, Swedish, and Dutch - which are all the languages the game has by default. You can improve the translation of an existing language by rewriting lines for that language in your mod. Any localization text given in a mod will replace the default line in the game when you have that language active.
  Your mod can also add entirely new languages! Just add a new entry with a unique language name, and it will appear in the Options menu as a new language option. For instance, this mod adds the fictional language of 'Lorem Ipsum' as a new language choice. It does this by adding the tag "<lorem> ... </lorem>" to every string key. Like so:

<string key='NEW_GAME'>
    <lorem> Lorum! </lorem>
</string>