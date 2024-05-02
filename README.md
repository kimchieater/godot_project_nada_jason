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

now call player_movement function inside the 
_physics_process function


![alt text](image-12.png)


now create a function play_anim(movement)

and get AnimatedSprite2D in a variable.

![alt text](image-13.png)

if movement that's passed in is 1 or true, 

then we're going to play anim.play('run')

else its gonna be anim.play('idle')

![alt text](image-14.png)

also you can create a direction variable in a global scope, 

and if the user pressed left or right, you can put 

anim.flip_h = false or true.

.flip_h method will flip the sprite based on the direction.


![alt text](image-15.png)

call play_anim function inside player_movement

![alt text](image-16.png)
![alt text](image-17.png)