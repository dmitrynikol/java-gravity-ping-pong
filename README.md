Welcome to Gravity ping-pong game
======================

     This is an example game that recreates the classic game ping pong but with my personal vision. I called it gravity ping pong. The game uses LWJGL(for graphics) and OpenAL(for sound effects) technology. Let's take a closer look at them.
     1) What is LWJGL?
LWJGL (Lightweight Java Game Library) provides developers access to different high performance crossplatform libraries. It provides not just a graphics binding but a binding to OpenAL(open standards sound system). In addition, it also gives you access to input devices. This means that your game could be controlled from a gamepad, all from one library. LWJGL provides it�s own keyboard handling objects, so we don�t need use for that AWT anymore. We can simple using Keyboard class. Drawing a sprite on the screen is identical to the JOGL. It�s very easy.
     2) What is OpenAL?
OpenAL (Open Audio Library) is a library for creation of a virtual world of sound. It easily combined with OpenGL 3D world and can very well be used to create games. The OpenAL API is designed to be cross-platform and easy to use.
     For more information, see:
- LWJGL Wiki 
- OpenAL for Android
- Game Engines and Libraries Using LWJGL
- LWJGL General FAQ
- OpenAL specification
     3) So let's look at the game!
What the goal of the game? Ping pong is one of the most famous games of the world. The game rules are very simple. You play this game with the arrow keys on your keyboard. Two players hit a ball back and forth using table tennis rackets(in the game it's simple rectangles with different colors). Points are scored when a player fails to return the ball within the rules. In my version of this game if player(from the left side) fails to return the ball, the surface is turning clockwise or vice versa by 10 degrees(it's a random rotation) and player rectangle is reduced, but the opponent rectangle is increased. But if the opponent misses the ball, the platform is rotated by 10 degrees and tends to the horizontal position. In the title of the window you can see current frame rate(FPS) of the game and the game score. That's it :)
     Controls: 
- Esc - quit game
- Enter - enable/disable fullscreen mode
- Arrow keys (up, down, left, right) or (W, S, A, D) - spaceship movement
     Audio:
The game has a background music and the sound of the collision. The magic of the sound was done using OpenAL.
Here you can find the package with implementation of the sound.
     4) My ideas how to improve the game? 
- Add Sprite/Texture to the game
- DIfferent collision object effects
- Draw a trajectory of the ball and the gradual disappearance
- More real physics based on some realtime physics engine
- Powerups or bonuses that will allow to add extra abilities to the player for some time as a game mechanism, they can help in difficult situations or add some dynamic scene to the gameplay
- Additional barriers during gameplay
- Ability to fire at enemy objects
     We are done. It's a simple example how to build a game with OpenGL. Here is the link to gravity ping pong game. Have fun with the code! 
