# EXPERIMENT 01 - ALP FOR 8086
Name :S.Sumyuktha Rani

Roll no :212220230050

Date of experiment : 09/09/2022

## Aim:
To write and execute ALP on fundamental arithmetic operations.

## Components Required: 
8086  emulator 

## Theory:
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.

## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	Run emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) 
3.	Write the code for the appropriate program for ADDITION, SUBTRACTION, MULTIPLICATION, and DIVISION operations 
4.	Compile the program and check for the errors 
5.	Run (once there is no syntax error) 
6.	Click OK to see/view the output of your program on the Emulator screen.
7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,

![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)

8.	Click on emulate to start emulation

![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)

9.	If no errors are found click on run and check the status of various flags in the flags tab as shown below

![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)

## Programs for arithmetic operations:

## Addition of 8 bit numbers
```
MOV SI,1200H
MOV CL,00H
MOV AL,[SI]
MOV BL,[SI+1]
ADD AL,BL
JNC L1
INC CL
L1:MOV [SI+2],AL
MOV [SI+3],CL
HLT
```

## Output:
![image](https://user-images.githubusercontent.com/75234991/190918052-e400bf3d-5ca3-49a4-a7d8-b80f84582da6.png)

## Subtraction of 8 bit numbers
```
MOV SI,1200H
MOV CL,00H
MOV AL,[SI]
MOV BL,[SI+1]
SUB AL,BL
JNC L1   
NEG AL
INC CL
L1:MOV [SI+2],AL
MOV [SI+3],CL
HLT
```

## Output:
![image](https://user-images.githubusercontent.com/75234991/190918277-17bd384b-34ae-49b6-96d2-973a40811551.png)

## Multiplication of 8 bit numbers
```
MOV SI,1200H
MOV AL,[SI]
MOV BL,[SI+1]
MUL BL
MOV [SI+2],AL
MOV [SI+3],AH
HLT
```

## Output:
![image](https://user-images.githubusercontent.com/75234991/190918404-4ba666d8-cd74-4dc3-9de3-0b52fc0f9e7a.png)

## Division of 8 bit numbers
```
MOV SI,1200H
MOV AL,[SI]
MOV BL,[SI+1]
DIV BL
MOV [SI+2],AL
MOV [SI+3],AH
HLT
```

## Output:
![image](https://user-images.githubusercontent.com/75234991/190918456-cd5d36aa-93e7-4587-b115-7cc66d385b02.png)

## Result:
Thus, ALP on fundamental arithmetic operations has been written and executed successfully using emu8086.
