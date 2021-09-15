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
- elevatorStop --> currentFloor === onPress() OR currentFloor === calledFloor()
- doorOpen --> currentFloor === onPress() || currentFloor === calledFloor()
- doorClose --> (elevatorUp = True || elevatorDown = True) && currentFloor !== onPress()
- Set doorAtDestination() --> elevatorStop and doorOpen and stays open for predetermined time
- Set onPress() --> button tells elevator what floor number was pressed and adds to array
- Set floorQueue --> array for floors selected. List order is done by order of onPress(). Spliced by if a different button is closer or calledFloor() is closer
- Set emerStop() --> emergency stop, overrides all previous and future commands and implements elevatorStop and doorClose
- Set calledFloor() --> tells elevator what floor passenger called it to and splices floor number into array
- Set elevaDirect() --> tells elevator to go up or down.
- isButtonSelected --> True or False
- buttonOn --> Turns button light on if isButtonSelected() === True
- Set floorLevel()  --> print currentFloor as elevator passes it or stops at it

