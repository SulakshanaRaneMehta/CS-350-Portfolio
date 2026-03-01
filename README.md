# CS-350-Portfolio
Portfolio artifacts for CS 350: Emerging Systems Architectures &amp; Technologies
Student: Sulakshana Mehta  
Course: CS 350 Emerging Systems Architectures and Technologies  
Assignment: Module Eight Journal Portfolio Submission  

## Overview
This repository contains two portfolio artifacts from CS 350 that best represent my work in emerging systems architectures and technologies. These projects demonstrate my ability to write interface software for hardware components, work with embedded-system style logic, and evaluate architecture choices based on technical and business requirements.

The two selected artifacts are:

1. Milestone3.py – Module Five Milestone Three: Input With Buttons  
2. Thermostat.py – Final Project Thermostat Lab  

I selected these artifacts because together they show both my programming skills and my ability to think about system design. One artifact focuses on state-machine logic and hardware interaction, while the second shows a more complete thermostat prototype with sensor input, display output, communication design, and architecture analysis.

---

## Artifact 1: Milestone3.py
This project focused on building an enhanced state machine that used LEDs and a button to transmit Morse code messages. In this milestone, I worked with a red LED, a blue LED, button input, and timing logic to create Morse code behavior for messages such as SOS and OK. The button allowed the system to switch between messages, while the state machine controlled the correct timing for dots, dashes, and pauses.

One important part of this project was learning why the LED blinking loop needed to run in a separate thread. Since Morse code requires exact delays, using a worker thread allowed the system to keep blinking the LEDs while still responding to button presses. I also learned the value of returning to the off state after each completed action so the system always returned to a clean and known state before the next signal.

This artifact reflects my ability to:
- use state-machine design in Python
- control hardware-related behavior through software
- debug transition and indentation issues
- apply timing logic carefully
- create a solution that is structured and easier to maintain

---

## Artifact 2: Thermostat.py
This project focused on building a smart thermostat prototype for SysTec using Raspberry Pi. The thermostat used an AHT20 temperature sensor, buttons, PWM-controlled LEDs, a 16x2 LCD, and UART communication. The state machine included three system states: OFF, HEAT, and COOL. The system measured room temperature, compared it to a user-defined setpoint, and then updated the LEDs and LCD display based on the current condition.

This project also required more than coding. It involved comparing three hardware architecture options—Raspberry Pi, Microchip, and Freescale (NXP)—to determine how well each platform could support the thermostat’s peripherals, Wi-Fi connectivity, memory needs, and business goals. I concluded that Raspberry Pi was the best platform for development and prototyping, while Microchip or NXP microcontrollers would be more practical for production because of lower cost and lower power use.

This artifact reflects my ability to:
- design software for embedded-system style behavior
- integrate multiple peripherals into one solution
- think about communication between device and server
- compare architecture options based on both technical and business requirements
- justify design decisions clearly

---

## Reflection

### Summarize the project and what problem it was solving
The projects in this course focused on how software can control hardware components and support embedded systems. In the Morse code milestone, the problem was to create a working state machine that could send messages accurately using LEDs and respond to button presses without interrupting timing. In the thermostat project, the problem was to create a prototype that could read temperature, manage heating and cooling states, display status information, and prepare for future cloud connectivity. Together, these projects helped me understand how software and hardware interact in practical systems.

### What did you do particularly well?
I think I did particularly well in organizing logic step by step and applying state-machine design carefully. In the Morse code project, I was able to connect button input, LED output, and timing rules in a way that supported accurate message transmission. In the thermostat project, I did well in combining several peripherals into one prototype and clearly explaining how different architectures could support the same business requirements. I also stayed patient through debugging and testing, which helped me complete the projects successfully.

### Where could you improve?
I could improve by spending even more time on testing, optimization, and code polish before final submission. Sometimes I needed extra time to fix transitions, wiring mistakes, or formatting issues, so I would like to become faster and more confident when troubleshooting. I would also like to improve my understanding of lower-level embedded programming so I can move more easily from Python-based prototyping into production-style microcontroller development.

### What tools and/or resources are you adding to your support network?
The tools and resources I am adding to my support network include Raspberry Pi documentation, Python libraries for GPIO and device control, sensor and LCD library documentation, state-machine diagrams, and GitHub as a portfolio platform. I also learned that visual diagrams, testing files, and step-by-step debugging are important resources when working on systems that combine software and hardware.

### What skills from this project will be particularly transferable to other projects and/or course work?
The most transferable skills from these projects are problem-solving, debugging, state-machine design, hardware/software integration, and writing organized code. These skills will help me in future embedded systems work, software development projects, and other computer science courses that require structured logic and careful system planning. I also gained experience in comparing technologies and making recommendations based on both technical needs and business goals.

### How did you make this project maintainable, readable, and adaptable?
I made these projects maintainable and readable by keeping the logic organized into clear sections, using structured state behavior, and following a predictable flow for transitions and hardware actions. Returning the Morse code system to the off state after each action helped keep the design easier to understand and debug. In the thermostat project, using a three-state structure and separating the responsibilities of input, control, display, and communication made the prototype easier to follow and adapt. I also used diagrams and written explanations to support the code and make the project more understandable for future review.

---

## Repository Contents
- `Milestone3.py`
- `Thermostat.py`
- Supporting assignment documents
- Supporting state machine diagram PDFs

---

## Closing Reflection
This course helped me better understand the relationship between software, hardware, and system architecture. It gave me practical experience with buttons, LEDs, sensors, displays, communication methods, and state-machine logic. These artifacts represent my growth in programming, debugging, and system thinking, and they show skills that I can carry into future coursework and technical projects.


