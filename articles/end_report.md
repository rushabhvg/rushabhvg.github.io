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

Firstly identify and address the obstacles with Rust Apps running on NuttX, which involved diagnosing issues related to compatibility, performance, or functionality.

The next goal was to implement Embedded Rust Apps in NuttX by writing and integrating code to ensure proper functionality. This included configuring the system (Physical Hardware: Ox-64 SBC and an emulator: QEMU), integrating the Rust toolchain, and verifying that the Rust Apps met necessary specifications.

The next goal was to update the NuttX community by preparing a presentation, discussing the findings so far, and demonstrating Rust Apps capabilities through the LED Blinky Rust App on an Ox-64 Single Board Computer (SBC).

Finally, the project involved developing and testing the LED Blinky Rust App, which included coding the application, driver files, and the configuration script, and then deploying it on the Ox-64 SBC, and testing on various architectures (RISC-V 32-bit and RISC-V 64-bit) using the QEMU emulator.

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

During the GSoC period I had firstly set-up the Ox-64 SBC. I had connected and verified the hardware components, installed the necessary software, and ensured that the NuttX OS and NuttX Apps were running fine. I had installed and booted into NuttX and made sure that the connnections were okay and working. 

Then, I had implemented Embedded Rust code like puts, printf, scanf, string formatting, etc. Since the Embedded Rust code was called from C, it was necessary that the data types in Rust properly matched with C's data types for smooth passing of data. Using this as a base, we have written the code for LED Blinky App in Rust. For calling the Open, IOCTL, Close, and other functions the Embedde Rust code was required. Using this LED Blinky App developed, we had given a presentation and a demonstration in the NuttX International Workshop.

After the workshop, we had written the LED and GPIO drivers for Ox-64 SBC. Since, these drivers were for RISC-V 32-bit and 64-bit architectures. And, since we can't use Rust cargo to install the dependencies, we have written a separate Rust package for the common file operations and input-output tasks. Using this package, we wrote the safer Rust LED Blinky App. Also, we have tested the application on RISC32-bit and 64-bit architectures using QEMU.

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
