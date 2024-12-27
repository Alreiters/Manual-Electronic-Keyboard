# Manual Electronic Keyboard

Electronic Design Program

@Author: J. X. PENG (Alreitetrs Pourton)

# I. Design Requirements and Analysis

1. Requirements
Press the matrix keyboard to drive the passive buzzer on the baseboard to produce different tones and play a piece of “Little Star” or music of your choice.

2. Requirement Analysis
Get the information typed by the matrix keyboard, then decode the output information of the keyboard into corresponding syllable data through encoding, and finally drive the passive buzzer on the baseboard to produce sound through the NE555 module.

According to the above requirements, it can be concluded:

(1). Design the matrix keyboard circuit to realize the signal acquisition and feedback.

(2). Acquire the input signal and decode it into the corresponding syllable data.

(3). Design the passive buzzer circuit driver board, through the NE555 driver to send out the corresponding frequency sound.

# II. Overall Design and Block Diagram
1. Overall realization scheme :

(1). Overall generalization

The design of the simple electronic piano is realized through the combination of hardware and software. The hardware system includes the master controller chip, the matrix composed of 8 keys, the buzzer and so on, and the software resources include Multisim, Litron EDA and so on. The electronic piano has the function of playing the keys instead of the keys and the function of automatic playback. 

(2). Detailed introduction

The whole program is divided into 2 modules: the main module and the key module. 

The whole program uses a total of 8 keys (key1~key8), which are used as keys to key in different scales.

The NE555 is used to generate a square wave:

![image](https://github.com/user-attachments/assets/7ccbcd7f-86a2-49c4-aad8-1de4c08e71f1)


2. Specific functional descriptions:

![image](https://github.com/user-attachments/assets/5151d3a4-96e3-453a-8f25-bf616f5bf5a5)


3. Top-level segmentation

![image](https://github.com/user-attachments/assets/8d8367a8-907d-4be1-b301-d2efbbb3be52)


4. Key Module

Function: Key in 8 different scales by key1~key8, the buzzer will sound differently with different frequencies.


# III. Designing Circuits in Modules, Simulation

![image](https://github.com/user-attachments/assets/3ab692a5-6787-4095-a88e-ae8cc1bfaaae)

![image](https://github.com/user-attachments/assets/475468fb-c98d-41d4-a127-4b3b43902099)

Signals:

Input signal: a clock signal, 8 keys;

Output signal: a buzzer output tone.


# IV. Experiment and debugging results
1. Hardware test results:
After the timing verification download , through the hardware test, the experiment achieves the expected results, through the key1~key8 the eight keys of the eight scales of sound that can be emitted by the buzzer, that is to say, it indicates the playing function of the electronic piano; through the test of the hardware, all the design objectives are realized.

2. The discussion of the problems of the results and conclusions:
In the process of experiment, the buzzer pronounces sound sometimes good and sometimes bad, sometimes it is low, but sometimes it is sharp, which may be the result of imprecise frequency division of the main system, when the main system clock is divided into different frequencies, the result is different, and finally, after many times of test, we get the most ideal effect under the frequency of 6M clock.

3. Tone scale and its corresponding frequency (clock frequency of 50 MHz is divided into 6 MHz)

![image](https://github.com/user-attachments/assets/1edb577a-039a-445f-ab0a-e090a7abf269)


# Attachments:
1. Circuit diagrams

![image](https://github.com/user-attachments/assets/609e5c50-843b-4673-8075-d619f416a67c)


2. Circuit board

![image](https://github.com/user-attachments/assets/57c8663f-73d8-46f6-9008-442c4bddfe3e)


3. PCB effect diagram
 
![image](https://github.com/user-attachments/assets/ed7b6843-e92b-4bef-86b7-5cedc99e2edd)

![image](https://github.com/user-attachments/assets/7025cdd3-e6d2-42e4-bfa1-62aae0b4e4bb)


4. Physical drawing

![image](https://github.com/user-attachments/assets/05236f2e-8cec-4dc2-ab9f-e367ca69eae8)

