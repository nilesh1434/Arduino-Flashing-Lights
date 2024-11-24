# Flashing Lights

This project is a memory game created using multiple Arduino UNO boards, involving a sequence of LED patterns that the player must memorize and replicate. The game uses wireless communication between different Arduino boards and provides interactive feedback through LEDs, an LCD display, and a buzzer. The game also includes a difficulty progression where the sequence length increases as the player successfully replicates the patterns.

---

## 📝 Abstract

The game displays a 2x3 LED light pattern that the player needs to memorize and replicate in the correct sequence. The project consists of four Arduino boards communicating wirelessly:
- **Master Board (Board 1)**: Displays the LED pattern.
- **Controller Board (Board 2)**: Accepts player input to replicate the pattern.
- **LCD Display Board (Board 3)**: Displays game information such as score and difficulty.
- **Buzzer Board (Board 4)**: Provides feedback on the player's actions.

---

## 📂 Project Structure

The project consists of the following key components:

1. **Master Board (Board 1)**:
   - Displays the LED sequence.
   - Increases difficulty by adding more LEDs to the sequence.
   - Communicates with other boards using Rx and Tx.

2. **Controller Board (Board 2)**:
   - Accepts user input (via buttons and joystick).
   - Sends the user’s input to the Master Board.
   - Adjusts the game difficulty.

3. **LCD Display Board (Board 3)**:
   - Displays game-related information such as difficulty, scores, and current player input.

4. **Buzzer Board (Board 4)**:
   - Provides audio feedback based on the player's actions, announcing correct/incorrect inputs.

---

## ⚙️ Components Used

- **Wires**: ~50
- **Resistors**: ~25
- **LED Lights**: 10
- **Buttons**: 5
- **Joysticks**: 3
- **LCD Displays**: 2
- **Potentiometers**: 2
- **Buzzer**: 1
- **Rx and Tx Transmission Wires**: 4

---

## 🛠️ Materials and Setup

### Step-by-Step Process to Build the Project

1. **Master Board Setup**:  
   - Start by assembling the Master Board, which consists of a 2x3 LED light pattern.
   - Set up Rx and Tx communication for connecting with the other boards.
   - Implement code to randomly generate a light pattern for the user to memorize.

2. **Controller Board Setup**:  
   - Assemble the Controller Board to accept user input via buttons and a joystick.
   - Test the joystick movement by lighting up test LEDs and sending data to the Master Board using Rx/Tx.

3. **LCD and Buzzer Setup**:  
   - Set up the LCD Display Board to show the current game state, including score and difficulty.
   - Connect the Buzzer Board to provide audio feedback based on game events (correct/incorrect input, winning/losing).

4. **Testing and Debugging**:  
   - Test the communication between the boards.
   - Ensure that the Master Board correctly handles inputs from the Controller Board and displays feedback on the LCD and Buzzer boards.

---

## 🚀 How to Play

1. **Start the Game**:  
   - The player can input their name using the joystick and buttons on the LCD board.
   - Press the "Start" button to begin the game on the Master Board.

2. **Memorize the LED Pattern**:  
   - The Master Board will flash a 2x3 LED pattern that the player must memorize.
   - The sequence length increases as the player successfully repeats the pattern.

3. **Replicate the Pattern**:  
   - The player uses the Controller Board to replicate the LED pattern by selecting the corresponding LEDs.
   - The Buzzer Board will provide feedback (correct or incorrect) on the player's selection.

4. **Game Progression**:  
   - The player moves through levels of increasing difficulty, with longer sequences to memorize.
   - The LCD Display Board will show the current score and difficulty level.

5. **Winning or Losing**:  
   - The game ends when the player either successfully completes all levels or fails to replicate a sequence.

---

## 📡 Communication Mechanism

- **Controller Board → Master Board**:  
  - The Controller Board communicates wirelessly with the Master Board via Bluetooth or Rx/Tx to send user input (button presses, joystick movements).

- **Master Board → LCD Display Board**:  
  - The Master Board sends information about the game state to the LCD Display Board, updating the score, difficulty, and user input.

- **Master Board → Buzzer Board**:  
  - The Master Board triggers the Buzzer Board to provide audio feedback (correct/incorrect responses, game status updates).

- **Master Board → LED Board**:  
  - The Master Board sends the LED sequence to the LED Board to display the pattern that the player must memorize.

---

## 🔧 User Guide

1. **Name Input**:  
   - Use the joystick on the LCD Board to select letters for the player's name. Click the button to input the selected letter.

2. **Game Start**:  
   - After entering the name, press the "Start" button on the Master Board to begin the game.

3. **Game Play**:  
   - Memorize the LED pattern that flashes on the Master Board.
   - Use the Controller Board to replicate the pattern by selecting the corresponding LEDs.

4. **Difficulty Adjustment**:  
   - The difficulty increases automatically as the player successfully memorizes longer patterns.
   - Use the button on the Controller Board to adjust the difficulty level if needed.

5. **Audio Feedback**:  
   - The Buzzer Board provides audio cues for correct or incorrect actions and announces game events such as winning or losing.<br><br>

Enjoy the game and have fun improving your memory! 🎮

Happy Coding!!!
