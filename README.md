EVM-8051-summer-training
========================
This is code for implementing Electronic Voting Machine in 8051. (For three parties only).
port P1.3-P1.5 are used as input
port P1.0-P1.2 are used as as LED port to indicate successfull input, and to blink LED 
corresponding to number of votes of party
port P1.6 listens to event to event corresponding to give results.

Label Delay: Produces delay for 2 seconds

Labels L1: Polls if any of input button are pressed

Labels M1,M2, M3 : give code to handle event on input press. Switches LED on to indicate successfull input for 2 sec.

label M1_1,M2_1, M3_1: to prevent counter of cotes from increasing if users keeps the input button pressed, by looping continuously within this loop .

Label M4_1 : Code invoked when port P1.6 set i.e results are to be displayed

Labels M4_1_1,M4_1_2,M4_1_3: Code invoked when ports P1.1,P1.2 and P1.3 set respectively. This code blinks LED attached to port P1.0,P1.1 and P1.2 respectively, corresponding to number of votes for each party.

Labels M4_1_1_1,M4_1_2_1,M4_1_3_1: code within slbels M4_1_1,M4_1_2,M4_1_3 to handle case when user keeps button on port P1.3,P1.4,P1.5 pressed while displaying results.

Label Loop_1,Loop_2,Loop_3: Contains code for blinking LED attached to ports P1.0,P1.1,P1.2 for displaying results. 
