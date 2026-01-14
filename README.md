Gaming Interface Assistive for the Visually Impaired

An embedded system prototype was developed to make the classic board game Snakes and Ladders accessible to visually challenged players. Built using Arduino C++, this project replaces visual cues with a tactile-audio feedback loop.
![setup image](https://github.com/user-attachments/assets/65263b7f-6808-41bd-944b-e4e0ee85e1d0)


## How it works
The unit monitors game states with state-machine implementations.
Tactile Inputs: Players get to press buttons situated at important places on the board (Snake's Head/Tail, Ladder Base/Top)
Audio feedback through an active buzzer gives the following Auditory Icons: A long beep at 1000ms indicates that a Snake or Ladder event has been initiated. A short beep at 500ms will validate that the player has reached the end of the move.
![game board](https://github.com/user-attachments/assets/61df68ee-e91c-4789-8971-1b2166462bac)




## Hardware Components
- Arduino Uno/Nano Microcontroller - Five Tactile Push Buttons as Inputs
- One Active Piezo Buzzer Output- INPUT_PULLUP is being used to keep the circuit small.
![arduino connections](https://github.com/user-attachments/assets/1b764d35-3bcf-496d-89a1-0d5fab26f7b3)

Software Feature
- Delays are integrated for debouncing so that there will not be any false triggering during tactile pressing.
- "Event" state tracking so that all moves have to be completed in sequential order.
