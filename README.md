# Arduino-Flashing-Lights

Abstract:

The project is a memorization game in which there is a 2x3 LED light pattern that is to be memorized by the player and then outputted in the same sequence from the controller board. Another board will have all of the necessary information such as a high score, difficulty, user info, displayed on a screen while the final board outputs sound according to the game events occurring. The project will communicate between all 4 boards to allow a user to progress between progressively larger sequences until the user fails.


Overall Description:

The project involves using the Arduino to display a sequential pattern of LED’s flashing as a memory game. It will use a form of Rx and Tx to communicate with another arduino board. The user then plays the game by trying to input the same pattern as the flashing led lights in the correct order to move on further in the game. For this idea we would need input devices such as switches to turn on the game when it is ready to take input from the phone as well as a button to adjust difficulty. We will use led lights as output devices to display the pattern, an LCD screen to show users the difficulty and a buzzer which will interact with the user depending on the inputs. What makes this project unique is the utility of wireless communication for a matching pattern game that would normally exist all on one single device. The purpose of the system is to create a fun and addicting game for all ages. The game uses a masterboard(1) with a 2x3 LED light sending information to the display(3) and buzzer(4) boards. These 2 boards are more for output purposes while the input comes from controller(2) board where the user provides input back to the board.
