# Circuit_Design

Circuitry Design of a Security Controller

## Objectives:

* Understand what you are being asked to do
* Use Logisim to implement the solution
* Design a test plan to verify the circuit functions correctly

## Tasks and Submissions:

* Submission options for the circuit are:
  * Live demo to instructor during lab zoom sessions
  * Live demo to instructor or TA – make appointment if out of lab sessions
  * Make a movie recording that shows you building the circuit (part of the circuit is OK) and shows you testing the circuit documenting all inputs and outputs. Submit in Canvas.
  * **Required also** : Submit the Logisim circuit (the *.circ *file) in Canvas
* Project report requirements:
  * A brief description of the design process you used to obtain the circuits. Be sure to point out why you chose a particular design, along with the steps you took to minimize the amount of hardware required. This includes
    * State diagram
    * State reduction
    * Final (reduced) state table
  * Include all design elements, such as truth tables, state diagrams, tables, etc,
  * Test the device in the simulator. Include a test plan:
    * Include your secret code for verification
    * Example inputs, expected outputs and what happened when you tested.
    * Descriptions, along with a detailed explanation of what simulations you did, what they show, to demonstrate that the circuit works properly under “all” circumstances.

**NOTE that all Logisim implementations **must meet all labeling requirements, as established at the []()start of the semester (see Lab 1)

## Project Description

There are many security and access control devices on the market that attempt to prevent unauthorized access to secured areas. One such device is a key-pad based device. To unlock the door, you must enter a secret decimal code. For example, say a device accepts a 4-digit decimal code, 1234. The device will unlock the door when “1234” is entered, but it will not unlock if “123” or “123411” is entered.

For your final project, you are to design an access control system based on a sequence of 6 bits that accepts a 1-bit at a time, either 0 or 1. This could be implemented with a 2-button keypad (o and 1), used to enter the binary code.

A second input functions as the *Enter *key, which ends the key code entry. As the key is entered, the device outputs Enter = 0 until the input sequence terminates. If the input sequence matches the

access code, then output Enter =1 (for example LED lights up), which will unlock the door in a full implementation. The secret code is preset: choose your own code (see below).

After two unsuccessful attempts (i.e. the secret code was not matched), the system shuts down and won’t accept any more bits, and an alarm is triggered. Thus, your circuit has a second output Alarm, which is set to 1 after two unsuccessful attempts.

Extra credit: Add a reset to the system that presumably only the owner could control: when the reset key is inserted, the system is again enabled and can accept bits again. You can code the reset as either 0 (no key) or 1 (key inserted) for this project.

Secret code:

* Each of you has their very own secret code: no 2 people in the class can have the same code
* Your code can NOT be a simple sequence of all 1s or all 0s, and must contain a minimum of 2 ones and 2 zeroes

For this final project, you are allowed to work together on design, but each student’s solution will be unique, because each of you has a different secret code.

Sign up for you code, be sure you are signed in to your TWU email account and access the shared [secret key code signup sheet](https://docs.google.com/spreadsheets/d/1zxFyoGbxKF6KTLkjCs-z31T4wlootW1h5B1IWsnBbl4/edit?usp=sharing "https://docs.google.com/spreadsheets/d/1zxFyoGbxKF6KTLkjCs-z31T4wlootW1h5B1IWsnBbl4/edit?usp=sharing")

A schematic of the device is shown in the figure below for a secret code of 8 bits..

![]()**Security Control Device**
