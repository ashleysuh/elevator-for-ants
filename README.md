# elevator-for-ants
2-story elevator as a finite state machine

Final project for USF's Computer Logic Design Lab:

Design and implement a finite state machine which controls the operation of an elevator in a
2-story building.

The finite state machine (FSM) has 1 input:
1. enable (enables operation of elevator)
The FSM has three outputs:
1. door (if door == 0, door is closed if door == 1, door is open)
2. Current floor number (display the current floor using a 7-segment display).
3. Moving (display that the elevator is moving)

The operation of the elevator is as follows:

** The elevator must begin in an idle state (on one of the two valid floors) with the door
closed.

** The user should set the enable input to move the elevator to the other floor. It is the
responsibility of the user to reset the enable input before leaving the elevator.

** When the user sets the enable input, the elevator should perform the following
sequence:
o Open the door for 4 seconds
o Close the door
o Move the elevator to the destination floor in 4 seconds and display the
current floor number using the 7-segment display
o Open the door for 4 seconds
o Close the door
o Remain in the same floor until the enable input is set again.

** Assume that the clock frequency is 4 Hz
