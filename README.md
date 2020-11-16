# Dodger

Dodger game on Uno32 Chipkit with Basic I/O Shield

Objective and Requirements:

Dodger is a game inspired by the likes of Snakes where you eat blocks of food that appear on the screen randomly all while trying to avoid ‘mines’ that also appear randomly on the screen. You get to control an 8 pixel (horizontal) by 2 pixel (vertical)  structure that is always moving rightwards, you control the structure by moving it up or down. The player gets 3 attempts or lives when playing the game, each obstacle collision reduces this by 1. The objective for the player is to last as long as possible while trying to eat the blocks of food that appear on the screen.

The game fulfills the following requirements:

The user controls the ‘Dodger’ with the push of two buttons on the ChipKIT board.
The user has an ability to increase the speed of the game with the push of a button.
Displays the high score at the end of each game session.
There are two different levels where the obstacles are of different shapes.
The LEDS dim one by one for every life the player loses.


Solution:

The project has been developed on the ChipKIT Uno32 board along with the Basic I/O Shield. All the code has been written in C. The small OLED display screen on the Basic I/O Shield has been used to display the game. When the user pushes Button 2, the Dodger moves up by 2 pixels and it moves down similarly when Button 4 is pushed. Pressing Button 3 increases the speed at which the Dodger is moving. The user inputs are taken as interrupts when the user pushes the buttons. The food blocks are 2 pixels by 2 pixels in size while the mines are 4 by 4 but do not fully light up the 4 by 4 square of pixels. The Dodger detects food or obstacle collision by comparing the pixels that it updates each time it moves, a visual demonstration of this will clarify things further. The OLED display has been utilized by following the ChipKIT Basic I/O Shield reference manual for the OLED Graphic Display section,Appendix B. 

