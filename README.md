# Arcade-Stick-Research-Project

This is my senior research project for building a custom "stickless" arcade stick controller. That means instead of having your classic arcade stick controls, the stick is replaced by up/down/left/right buttons.

This project made me do research create many first times for me related to PCB creation, Arduino coding, and 3D printing.

## Table of Contents
- [Motivation For This Project](#motivation)
- [Project Overview](#overview)
- [Features](#features)
- [Hardware and Software Architecture](#architecture)
- [Prerequisites](#prerequisites)
- [Building](#building)
- [Future Improvements](#improvements)

## Motivation For This Project
Starting early in high school, I always went out and competed in games like Super Smash Bros. and Street Fighter, so I've always had a connection to the scene. I've built controllers for myself with kits, but I wanted to take a crack at actually creating one from scratch.

I also enjoy embedded systems, and wanted to have my project focus on more hardware than software so that I could gain more experiencce working in this subject.

## Project Overview
My arcade stick is a custom controller project combining PCB creation, 3D printing, microcontroller firmware, and supprot of PC software. The goal of this project is to have a fully functional stickless controller that can be used to play fighting games on PC.

## Features
- Custom hardware: I designed the controller shell, buttons, and PCB for complete control over the hardware and software
- Gamepad emulation: using the Arduino keyboard library, you are able to emulate a gamepad to be recognized as a keyboard.

## Hardware and Software Architecture
Hardware:
- Microcontroller: Arduino Pro Mini
- Buttons: uses Charry MX Switches with 3D printed buttons based on 30mm arcade buttons
- PCB: custom PCB designed to be like a keyboard with rows and columns for optimal button pressing and space 
Firmware:
- Custom microcontroller code that reads button inputs from the PCB and translates them to keyboard inputs

## Prerequisites
- Arduino Pro Mini
- Cherry MX Switches
- USB C cable
- Forward bias diodes

All printing and PCB files are listed in this repository.

## Building
1. Solder Arduino, switches, and diodes (always pointing down)
2. Place PCB in controller shell
3. Plug controller into PC and compile code onto it from Arduino IDE
4. Now you're set to start playing!

## Future Improvements
1. I originally wanted to have this controller use Xinput instead of acting as a keyboard, but I was having compiling issues with my specific Arduino. In the future I would like to switch to a different microcontroller that better suites what I want.

2. I also considered adding features onto the controller to be able to work on Xbox, Playstation, and Switch. It was already enough with figuring out the hardware side of this project, so I didn't have the time to research the communication protocols of these console and how I could implement them onto my controller.

3. I would like to optimize the controller shell to either be smaller for better travel, or bigger and better ergonomics for playing as this controller felt a little too box-like.
