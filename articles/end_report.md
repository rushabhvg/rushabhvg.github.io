#GSoC Final Report

***************************** Just a draft and not the final report *****************************

Hello! Welcome to my blog about my experience with GSOC 2024 mid terms!

# Introduction
I am Rushabh Vipul Gala, studying Computer Science and Engineering at the University of Mumbai, India. I love to solve real-world challenges, and want to contribute for the betterment of the world. I have a keen interest in new technologies. And I am thrilled to be able to contribute to the Open Source Community through Google Summer of Code (GSoC).

# A short description of the goals of the project
The main goals were to:
- Identify and Address obstacles with Rust and NuttX
- Implement embedded Rust in NuttX and NuttX Apps
- Update NuttX folks about Rust in NuttX thorugh NuttX International Workshop
- Develop and Test drives for LED Blinky App in NuttX for various architectures

# What you did
What I did mainly is:
- Configure and Set-Up Ox64
- Install and Boot NuttX on Ox64 SBC
- Implement Embedded Rust
- Write application code for LED Blinky App in Rust based on C
- Gave a demonstration on Ox64 SBC in NuttX International workshop
- Resolved some queries regarding Rust Cargo through the workshop
- Developed LED and GPIO drivers in C for Ox64 platform
- Developed a safer version of LED Blinky App
- Tested on QEMU RISC-V 32-bit and 64-bit
- Create a Rust package for all some unsafe operations (OPEN, IOCTL, PUTS, etc)  

# The current state
- Currently, we have tried our best to identify and resolve the issues related to Rust in NuttX community
- Successful demonstration at Workshop and resolved querries related to Rust Cargo
- Implemented embedded Rust functionalities in NuttX 
- We now have a Rust package which can be used to develop applications in the future
- LED and GPIO drivers for Ox64

# What's left to do
- ***************************** Please guide here *****************************

# What code got merged (or not) upstream
- Mostly all the code got merged
- TODO: Listing all the PRs and their short summary
- Few functionalites of embedded Rust implemented through LED Blinky App didn't got merge in `hello_rust.rs`
- A new applcation with new configuration files was made: `leds_rust_main.rs`

# Any challenges or important things you learned during the project
- I faced many challenges as mentioned in previous post (listing those issues in brief)

# Things I learnt:
- Task Priortisation is important while handling deadlines
- Documentation may take time but it's important
- How to write a good PR
- I may not always be the best
- Open source is all about learnings and improvements rather than perfection
- A good mentor can help even a newbie become Beginner to Intermediate developer

# QnA with my mentor Mr. Lup Yuen Lee
(All the 3 questions and answers)
