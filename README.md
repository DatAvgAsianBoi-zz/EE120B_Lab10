# EE120B_Lab10

This repo contains the source code for the implementation of concurrent synch state machines in C for Lab 10 for EE120B taken at UCR in spring 2020.

For Part 1:
In one state machine (ThreeLEDsSM), output to a shared variable (threeLEDs) the following behavior: set only bit 0 to 1, then only bit 1, then only bit 2 in sequence for 1 second each. 
In a second state machine (BlinkingLEDSM), output to a shared variable (blinkingLED) the following behavior: set bit 3 to 1 for 1 second, then 0 for 1 second. 
In a third state machine (CombineLEDsSM), combine both shared variables and output to the PORTB.

For Part 2:
Modify the above state machine so the threeLEDs light for 300 ms, while blinkingLED’s LED still blinks 1 second on and 1 second off.

For Part 3:
Updating the previous exercise's implementation, connect the speaker's red wire to PB4 and black wire to ground. Add a third task that toggles PB4 on for 2 ms and off for 2 ms as long as a switch on PA2 is in the on position.

For Part 4:
Extended the previous exercise to allow adjustment to the sound frequency up or down using buttons connected to PA0 (up) and PA1 (down). Using our 1 ms timer abstraction, the fastest we'll be able to pulse is 1 ms on and 1 ms off (500 Hz). 
