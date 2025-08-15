# Smart Foosball Scoreboard

This repository contains the code for a smart foosball scoreboard that has two player mode and single player mode functionality. 

## Project Overview

- **Two player mode:**  
  - Uses photoelectric sensors for goal detection and a buzzer for feedback
  - Utilizes a button for each seven segment display so the user can manually increment score   
  - Includes a reset button to restart the game
  - Upon holding the reset button (set for two seconds) the game will transition to single player mode indicated by blinking of the seven segment displays 

- **Single player mode:**  
  - Uses the left photoelectric sensor for user goal detection and a buzzer for feedback
  - Right button starts computer scoring simulation
  - The system scores a point on the right seven segment display at random times within the set interval to simulate a real life opponent - buzzer sounds off upon system goal
  - Contains score reset functionality
  - Transitions back to two player mode upon holding the reset button (set for two seconds) indicated by the blinking of the seven segment displays 
  - First to 10 wins - victory blinking indication included

- **Hardware platform:** MSP430F5529 LaunchPad
- **Important Hardware:** 2x 74HC595 shift registers (chained), 2x seven segment displays, 3x buttons, 1x buzzer, 2x photoelectric sensors 
- **Source files:** All code is located in the `src/` folder



