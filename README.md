Intro programming - Report
=======================
MA Computer game art and design
KunAn, Li
33410075

----------
Programming isn’t something that people can master in an hour, but through around one month transition on taking this module – Intro to game programming, I begin to appreciate the magic of it in making video game and have a preliminary idea of how it works at many helps from Raul, Alejandro, Tin and other friendly classmates.  The knowledge of programming that I have chance to peek are including understanding working environment, how certain words work in programming and also nailing the tasks we been asked to do in example invaderer. Hence, in the following text I will demonstrate how much I understand in the programming area via examples Andy provided.




First of all, though, I have experiences in making indie game while taking undergraduate, it is my first time to hear Visual Studio and GitHub. Visual Studio is an integrated development environment which often use to develop computer programs and in our case is for game developing. Aside from that, it supports various programming languages and debug systems to adapt different code editors. Moreover, Visual Studio can work along with Unity to enhance game developers accuracy and productivity in coding. On the other, GitHub is an online repository service for source codes. It offers private repositories and free accounts to allow users collaborate together in remote location. 




Secondly, by looking into the example – invaderers understand that to make a basic 2D game programming we need to initialize the several settings first for game environment for example, camera, borders, shade, objects, array,CSV files. In addition, afterward we need to add functions to call them into main scene while needed events to interact such as making ‘for loop’ to draw sprites, ‘if’ to detect whether sprites clash to the border and timer to count whether objects should be added or removed.




*Followings are the modifications I made in example – invaderers:*
==

### 1.	Key down ‘2’ to add number of players’ life
- Adding one function by ‘if loop’ while KeyDown to increase the number of life. 


### 2.	Greatly decrease the interval time of missiles
-	Change the original missile function from key_going_down to key_down and make the time missiles_disabled shorter to make missiles continual firing.

### 3.	Replace whoosh sound to laser sound.
-	By switching the original wav file in the asset file to another free source laser sound.

![A001](https://raw.githubusercontent.com/kunanli/octet/master/octet/assets/exam03.jpg)

### 4.	Replace images of spaceship and sprites.
-	By switching the original images file in the asset file to other source images.
### 5.	Add KeyUp and KeyDown to remote spaceship freely.
-	Duplicate the original coding for moving ship left and right, then change the number of movement direction and also apply KeyUp and KeyDown to that.

### 6.	Apply solid colour shader on all object on the scene.
-	Open texture_shader.h which is inside the shader folder, and find the source code which affect the colour of all objects in invaderers.
-	Learned how to use binary code to change its RGB or UV color.
   
### 7.	Add Big Boss after killing all the sprites
-	Create a place for putting the boss.
-	Set the boss with source image, size, and location.
-	Turn off the gameover while all of the sprites dead.
-	Call the boss into the scene by transiting the location.


### 8.	Create life, missiles collision and score on BigBoss
-	Add number of boss life
-	Create a loop if missile hits the boss, then the hp will decrease 1 and score++, if number of life is zero then game over. 
![A001](https://raw.githubusercontent.com/kunanli/octet/master/octet/assets/exam02.jpg)

### 9.	Boss move and collide with border
-	Create a function to define the translation of the boss in float parameter. 
-	Add initial boss velocity
-	Add a function to confine the boss inside the game scene and increase its velocity when everytime it hits the border.
-	Draw the boss 

### 10.	Change background colour to white
-	Initialize the background colour into white by binary colour coding.

### 11.	Read CSV file and apply it on changing sprite colour
-	Create a string buffer to put the values in CSV file
-	Read the values in stream
-	If loop to detect if the file exist and read until the end of the file.
-	Make pointers loop (column, character) to point the specific value in the Cell.
-	Build two ‘for loop’ to stand for num_rows and num_cols
-	Add ‘If’ event to decide whether the value in CSV is 0, if yes then presents the invaderers’ texture to ben.gif, else shows blueben.gif instead.

### 12.	Fireball effect with timer after transfer the position of sprites.
-	Make an array of fireball outside of the scene
-	Replace the sprite to fireball while hitting the sprite.
-	Set a timer for fireball, after running out the time, the fireball goes back to its original place.

![A002](https://raw.githubusercontent.com/kunanli/octet/master/octet/assets/exam01.jpg)


Conclusion
====
The several features have been added in the example – invaderers including the task we been told to do ;changing the shader and setting up sprites by reading CSV file.  t was very good opportunity to learn how programmer communicates with computer and understand computer logical thinking.  Finally, I would like to thanks Raul, Alejandro, Tin and other friendly classmates again, they really spend a lot of time to explain each line of code and fundamental coding knowledge to help me get into real programming.