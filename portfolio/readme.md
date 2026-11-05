#When modding this file to be another theme, here are the specific places that should change to keep the core functions working

#index.html
1. <head> Title
2. <head> Author: PLease keep myself as author and add yourself as modifier, also keep any credits to ZIM as they are the framework being used
3. Update head comments
4. <head> Title (inner <head>, see known problems)
5. <style> {body} background-image : (insert relative url), fix alt
6. <div> "bugLeft" -> change to custom character image, fix alt
7. <div> "story" -> change to custom origin story and goals
8. "rules" -> keep the dynamics the same, change what icons being used
9. "button" -> change label on button to fit theme
10. update any colours in <style> css, to fit theme
11. address on bottom is for original creator, please keep and just add self as modifier

#game.html
1.<head> Title
2. <head> Author: PLease keep myself as author and add yourself as modifier, also keep any credits to ZIM as they are the framework being used
3. Update head comments
4. "bugFiles.push" -> change concatenation of file names to match your own. Suggest keeping the name + number set up, as used later on in a loop. This particular batch of images are what the character is trying to avoid when they are running through the environment. Will give the character a -5 seconds (per this setup) if it comes in contact with them.
5. array[] Frame -> update files appending the bugFiles to match rest of images used in gameplay.
6. //the background, const x (currently const ram)
7. //move the background, change to your const x
8. BELOW //make badcode, in:
    //how often do the badcodes come, and how fast 
    -> change to your icon for time ups
9. //make the bug -> change to image of your character
10. //game over -> add name as modifier

#MECHANICS
1. If you want to adjust the length of time your charcter ran move throught the
environment, in game.html: //make a timer -> time: x (in real seconds)
2. Adjust speed of objects coming towards character in:
    //how often do the modules come, and how fast
3. There is an array called badcode[] (//make badcode) that is where the icons that give time to the character are stored. 
4. IF YOU CHANGE ANY OF THE VARIABLE NAMES TO MATCH YOUR THEME - you will have to refactor the code to match as they are used throughout the pages and it will break. Easiest, just change images, keep names the same.
5. Use .png files with no backgrounds with best results
6. Smallest an image should be is 450*450 pixels
7. Largest an image should be is 1050*1580 pixels

#KNOWN PROBLEMS
1. There are two <head> tags in index.html, if I remove the inner <head> the program breaks. Don't remember why it was set up that way but am keeping it since it breaks otherwise. 
2. Not a problem - a NOTE, but the image on the sides of index.html are mirrored, via <style>, imgRight;
3. Keep in mind, file names are bug themed, if you update one to match your theme you must update them all
4. If your images are too big the game won't work right