# EXPERIMENT--01-ALP-FOR-8086
### Name : SHYAM S
### Roll no : 212223240156
### Date of experiment : 18.08.2025





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition of 16 bit ALP (Register Mode)
```
MOV AX,1A52h

MOV BX,32B3h

ABB AX,BX
```

## Output

<img width="1920" height="1080" alt="Screenshot (82)" src="https://github.com/user-attachments/assets/f8c49b29-e0da-4a57-9294-199f0d97bace" />

## Subtraction of 8 bit numbers ALP (Immediate Mode) 
```
MOV AX,1a52h

SUB AX,32b3h

ret
```

## Output

<img width="1920" height="1080" alt="Screenshot (84)" src="https://github.com/user-attachments/assets/8e916476-4bc7-472c-96da-5164b781ae03" />

## Multiplication alp (Direct Memory Mode)
``` 
NUM DW 1a52h
           
MOV AX,32b3h

MUL NUM

ret
```
## Output  

<img width="1920" height="1080" alt="Screenshot (86)" src="https://github.com/user-attachments/assets/d5b64f89-0bca-437d-a070-cb9e6fbe9b6d" />


## Division alp (Register Indirect Mode)

```   
NUM DW 32B3h
           
MOV BX, OFFSET NUM 

MOV AX, 1A52h

DIV WORD PTR [BX]

ret
```
## Output  

<img width="1920" height="1080" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/071d9b8c-bd9b-4510-bb5d-bcce808b0ebe" />

## AND  of 16 bit ALP (Register Mode)
```
MOV AX, 1A52h

MOV BX, 32B3h

AND AX,BX

ret      
```

## Output

<img width="1920" height="1080" alt="Screenshot (88)" src="https://github.com/user-attachments/assets/89f616ce-20f2-4be9-8785-8f445e632c90" />

## OR  of 16 bit ALP (Register Mode)
```
MOV AX, 1A52h

MOV BX, 32B3h

OR AX,BX

ret       
```

## Output  

<img width="1920" height="1080" alt="Screenshot (89)" src="https://github.com/user-attachments/assets/108dc897-e0ae-45b2-8e5c-a69e9e24cb3e" />

## NOT  of 16 bit ALP (Register Mode)
```
MOV AX, 1A52h

NOT AX

ret      
```

## Output  
<img width="1920" height="1080" alt="Screenshot (91)" src="https://github.com/user-attachments/assets/b0bf1440-0ff3-4adb-9378-33ed7b3d9f91" />


## XOR  of 16 bit ALP (Register Mode)
```
MOV AX, 1A52h

MOV BX, 32B3h

XOR AX,BX

ret   
```

## Output  

<img width="1920" height="1080" alt="Screenshot (90)" src="https://github.com/user-attachments/assets/65ed7905-38d6-45ac-8cb6-1cd9c8d0840f" />

## Result :

The execution of ALP on fundamental arithmetic and logical operations is successfully completed.
