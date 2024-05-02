# godot_project_nada_jason


Duty

1: find assets
2: create system design
3: animation
4: mapping
5: basic script (movement, attack, HUD)

Thu 2 May


![alt text](image.png)

Once you started the project, It is a good practice to organise your files.


![alt text](image-1.png)

Now create a 2D scene, name it world, then save it to scenes folder.


CREATING A PLAYER

now create another scene, select the other node, and select CharacterBody2D, name it player.

tip : note that if you crate CharacterBody2D scene, you need to attach 2d collision node, AnimatedSprite2D


![alt text](image-2.png)

Click animatedSprite2D and go to Sprite Frames

![alt text](image-3.png)

![alt text](image-4.png)

![alt text](image-5.png)

click this and import assets.

![alt text](image-6.png)

Match the grid.

Now to make the player character more clearly 

You need to go to project - project settings - rendering - textures - Default Texture Filter to Nearest.

![alt text](image-7.png)

now lets add more.

Challenge add more animation based on the assets you've been given. 

now that you've created all the animation,

create  a script for player scene.

create two functions 

one _phtsics_process

two player_movement

create a variable named SPEED and give value to it.

![alt text](image-10.png)

and make sure to call move_and_slide() built in function.

![alt text](image-11.png)

You can also change the input map under project setting.

