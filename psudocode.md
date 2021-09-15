# Pseudocode for an Elevator System.

---
## **Goal:**
**-** Travel up and down required floors
###Objectives
- Go up a floor when needed.
- Go down a floor when needed
- Create an order on which floors to stop at
- Be able to call the elevator to the floor you're on
- Emergency stop
- Emergency help
- Mention which floor the elevator is on
- Give an option to Extend the time the door is open

---
## Objects:
- Elevator: Goes up or down the designated floors.
- Doors: Open when arrived at destination. Stay open for period of time to let people in or out.
- inButtonPanel: array of floors to choose from, an Open doors, an emergency stop and emergency call button
- outButtonPanel: has an up and down button.
- Displays current floor as elevator moves or idle.
## Defining functions:
- currentFloor --> Prints the floor the elevator is on
- elevatorUp --> currentFloor+=1
- elevatorDown --> currentFloor-=1
- elevatorStop --> 