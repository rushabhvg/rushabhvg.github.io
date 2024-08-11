# GSoC Final Report

`***************************** Just a draft and not the final report *****************************`

Hello! Welcome to my blog about my experience with GSOC 2024!

## Introduction
I am Rushabh Vipul Gala, studying Computer Science and Engineering at the University of Mumbai, India. I love to solve real-world challenges, and want to contribute for the betterment of the world. I have a keen interest in new technologies. And I am thrilled to be able to contribute to the Open Source Community through Google Summer of Code (GSoC).

## A short description of the goals of the project
The main goals were to:
- Identify and Address obstacles with Rust Apps in NuttX
- Implement Embedded Rust Apps in NuttX
- Update NuttX Community about Rust Apps in NuttX through NuttX International Workshop
- Develop and Test the LED Blinky Rust App in NuttX for various architectures

## What you did
What I did mainly is:
- Configure and Set-Up Ox64 SBC
- Install and Boot NuttX on Ox64 SBC
- Implement Embedded Rust for NuttX
- Write application code for LED Blinky App in Rust based on C
- Gave a demonstration on Ox64 SBC in NuttX International workshop
- Resolved some queries regarding Rust Cargo through the workshop
- Developed LED and GPIO drivers in C for Ox64 platform
- Developed a safer version of LED Blinky Rust App
- Tested on QEMU RISC-V 32-bit and 64-bit
- Create a Rust package for all some unsafe operations (OPEN, IOCTL, PUTS, etc)  

## The current state
- Currently, we have tried our best to identify and resolve the issues related to Rust Apps in NuttX
- Successful demonstration at Workshop and resolved querries related to Rust Cargo
- Implemented Embedded Rust App functionalities in NuttX 
- We now have a Rust Module which can be used to develop NuttX applications in the future
- LED and GPIO drivers for Ox64 SBC are now usable
- LED driver for QEMU RISC-V are is now usable

## What's left to do
- TODO: We'll discuss at the Monday Meeting

## What code got merged (or not) upstream
- All of the code got merged
- TODO: Listing all the PRs and their short summary
- A new application with new configuration files was made: `leds_rust_main.rs`

## Any challenges or important things you learned during the project
- I faced many challenges as mentioned in previous post (listing those issues in brief)
- TODO: Insert the link

## Things I learnt
- Task Priortisation is important while handling deadlines
- Documentation may take time but it's important
- How to write a good PR
- I may not always be the best but learning is important
- Open source is all about learning and improvements rather than perfection
- A good mentor can help even a newbie become Beginner to Intermediate developer

## QnA with my mentor Mr. Lup Yuen Lee
(All the 3 questions and answers)
