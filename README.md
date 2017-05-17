# ProfilePicture
1. set up this sketch on your local machine. it has an image with it, so the process is a little different than usual:
   - click the green `Clone or download` button from this repo main page
   - click `download zip`
   - unzip the file into your sketchbook folder (where you store your processing sketches)
   - here is a visual of what things should look like (but with different file/folder names):
   [img](https://raw.githubusercontent.com/WoodstockCS/cp/gh-pages/processing_folders.PNG)
1. open the sketch and fill in the blanks (there are 5 blanks near the middle of the code). it will take some noodling to figure out what goes in the blanks.
1. run the sketch, and press the spacebar to toggle between your sketch and the source image.
1. time to make some changes and see what happens. run your sketch between each of these changes:
   - tinker with the cellSize and scale
   - comment out the `float size = ...` line and add a new line `float size = cellSize * scale * .8`, then adjust the `.8` a bit
   - replace that `.8` (or whatever number you settled on) with `noise(x, y)`
   - comment out that `float size = ...` line and add a new line `float size = map(greyness, 0, 255, cellSize * scale, .5)`
   - comment out the `ellipse(...)` line and add new lines: `textSize(cellSize * scale);` and `text(txt.charAt(currentLetter), xLoc, yLoc);`
1. save a picture of yourself (or a stand-in) in your data folder
1. make the necessary changes to your code so that your picture is displayed instead of the bee:
   - change the `imageLoad` function call so it uses the filename of your picture
   - change the imgWidth and imgHeight variables so they are correct for your image. (HINT: check the println function in your code)
1. settle on some adaptations from above that you like, by uncommenting and commenting code, and tweak variables to make it unique.
1. when the sketch is running, press the `s` key to save a snapshot of your picture to your sketch folder
1. fork this repo, paste your code into the pde, and upload both (a) your saved (filtered) image into your sketch (the main) folder, and (b) your source image into the data folder.
