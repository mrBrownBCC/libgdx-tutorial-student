# LibGDX Tutorial

### Project Goals
1. Learn about development with the libGDX library
2. Learn how to deplpoy projects to github pages
3. Create the 

### Example Project

[Vist a completed version of the project here](https://mrbrownbcc.github.io/libgdx-tutorial-SOLUTION/)

### Setup Steps:
1. To test, you will need to forward port 6080, similar to other projects. 
2. Click the link below and keep open in another tab. It contains the initial instructions

### Additional Resources:
[Project Tutorial](https://libgdx.com/wiki/start/a-simple-game)
[https://libgdx.com/wiki/](https://libgdx.com/wiki/)

### Core requirements
1. Functioning version of the bucket game as shown in the tutorial. 
2. Addition of score printout that increases when water is added to the bucket.
3. Addition of fireballs or some othere negative object to the game. When it collides with the bucket, score should go down. 


### Programming Instructions:
1. Follow the instructions in the link above. I STRONGLY recommend working step by step, testing often. Make sure you understand each portion before moving on.
2. Change the coordinate system to be 800x500 instead of 8x5. This will allow text in the next step. Be sure to change all sizes and speeds by a factor of 100. 
3. The next few steps are for adding text. First, add the following import: 
import com.badlogic.gdx.graphics.g2d.BitmapFont;
4. Add the following instance variable to class Main: 
    BitmapFont font;
5. Add the following initialization in the create() method:
        font = new BitmapFont();
6. To print the text, add the following to the draw method (before spriteBatch.end()):
        font.setColor(Color.BLACK);
        font.draw(spriteBatch, "YOUR TEXT HERE", x, y);
7. Add a score variable to your game,  starting at 0. It should be printed in the font.draw command. 
8. Make score go up when a water drop collides with a bucket.
9. Find an image for the fireball. png is recommended. Add to the assets folder. 
10. Look at the code controlling water droplets. Add similar code for fireballs, adding an obstacle to avoid
11. Decrement score if the bucket collides with a fireball. 



### Testing:
To test your code, interact with the GUI you create! 

To test 'desktop version', use the following terminal command: 

./gradlew lwjgl3:run

NOTE - to do this you must have turned on port forwarding of port 6080

*Sound effects may not be testable with this method*

### Deploying
Now you can share your project with the world!
You will also need to complete this step before submission. 
Run the following two commands in the terminal:

NOTE - build may take 1-3 minutes. 

1) npm run build
2) npm run deploy 

*NOTE - the first time you deploy, it may take up to 10 minutes for the site to exist.* 
You now have a github pages available!
To find the link for your project- 
1. Go to github.com to double check your username and repo name. 
2. The URL for your project is:

https://<your-username>.github.io/<repository-name>/


### Submission:
Run the following 3 commands in the terminal:
1) git add . 
2) git commit -m "Submitting my code"
3) git push

Then, **ON CANVAS**, please submit the link to your github pages site. This link should take the user to a playable version of the game. 