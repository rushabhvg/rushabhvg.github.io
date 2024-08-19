# GSoC Final Report

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
- [Fix the Rust and D Builds for QEMU RISC-V](https://github.com/apache/nuttx/pull/12854)
- [Add Rust Target for QEMU RISC-V 64-bit](https://github.com/apache/nuttx/pull/12858)
- [Add Build Config for leds64_rust](https://github.com/apache/nuttx/pull/12862)

## What code got merged (or not) upstream
- All of the code got merged
- [Added GPIO Driver for Ox64 SBC](https://github.com/apache/nuttx/pull/12571)
- [Added LED Driver for Ox64 SBC](https://github.com/apache/nuttx/pull/12614)
- [Added LED Driver for QEMU RISC-V 32-bit and 64-bit](https://github.com/apache/nuttx/pull/12762)
- [Added Rust App for blinking the LED](https://github.com/apache/nuttx-apps/pull/2462)
- A new application with new configuration files was made: `leds_rust_main.rs`

## Any challenges or important things you learned during the project
- I faced many challenges as mentioned in the [mid-term report] (https://github.com/rushabhvg/rushabhvg.github.io/blob/master/articles/mid_term_blog_post.md)
- NuttX and NuttX Apps can't be built using Cargo. Hence, we had to make and build Rust Apps without Cargo.
- Enhanced my skills in Programming in C, Rust and Scripting.
- Learnt various standard practises of coding and programming in general
- How to create a good PR (Pull Request)
- And along all these things, my mentor Mr. Lup Lee Yuen, an experienced developer and a retired professor, has taught me countless small advices and tips to become a better programmer.

## Things I learnt
- Task Priortisation is important while handling deadlines
- Documentation may take time and it's curcial for the future development
- How to use Git and GitHub using Command-line and the Desktop Application.
- I may not always be the best but learning is important
- Open source is all about learning and improvements rather than perfection
- A good mentor can help even a newbie become Beginner to Intermediate developer

## QnA with my mentor Mr. Lup Yuen Lee
1. Think of a NuttX Developer, creating a NuttX App in Rust for the very first time. Have we done enough to help them? How else could we have helped?
Ans. Yes, we have enought to help an experienced NuttX Developer to create a NuttX App in Rust. Although, they might face difficulties in understanding the Rust Syntax, with time they should be able to easily understand Rust. We have developed and coded many NuttX POSIX APIs in Rust, which will help them in abstracting the underlying Unsafe code. There's still a small room for improvement and developing more such APIs.

1. In the First Half of GSoC, we ran Rust Apps on Ox64 BL808 RISC-V SBC. In the Second Half, we ran Rust Apps on QEMU RISC-V. Why was it necessary to do both?
Ans. Yes, we ran Rust Apps on Ox64 BL808 RISC-V SBC in the first half because NuttX and NuttX Apps are real-world applications, which are better to build, run, and test on a physical hardware to resolve any errors or glitches in the code. Since, not everyone has an Ox64 BL808 RISC-V SBC, and it's difficult to run the App on each existing Hardware, we had built, ran, and tested the Apps in QEMU RISC-V emulator, to make sure the Apps works on other architectures too.

1. Which topics should NuttX Project explore for the next GSoC? Create more NuttX Apps or NuttX Drivers (like for Ox64 BL808 SBC)? Or should NuttX Project collaborate directly with universities, and work on team-based projects?
Ans. There are many topics that NuttX Project could explore for the next GSoC, such as NuttX support for other platforms, creating more NuttX Apps for showcasing the capabilities of NuttX OS and the Community, or maybe a deep and thorough cleaning of the NuttX Codebase and Documentation. And, I believe it would be better to create more NuttX Drivers, which will enable more developers to create various Apps relying on the NuttX Drivers. I think, it's a good idea to collaborate directly with the universities to work on team-based projects. This will help the NuttX community to get new developers and the ideas they come up with. I think it's also beneficial for the students to learn and code in the standard way using Git.

## Acknowledgments

I am also thankful to Mahadev, Bhagwan Vishnu, and all the gods and goddesses for granting me this opportunity and guiding me through this journey.

I am incredibly grateful to Mr. Lup Yuen Lee for his continuous support, patience, and invaluable guidance throughout the GSoC. His expertise as an experienced developer and as a professor were very helful in shaping my understanding and skills in embedded systems as a novice student developer.

A special thank you to the Apache Software Foundation for providing me with this amazing opportunity to participate in GSoC. The resources and community at the Apache Software Foundation were essential in helping me achieve my goals and grow as a developer.

I am also grateful to PINE64 for sponsoring me with two Ox64 Single Board Computers featuring the Bouffalo Lab BL808 RISC-V SoC, along with the setup tools. These resources were essential for testing my code and applications on physical hardware for the first half of the GSoC and sometimes in the second half.

I extend my thanks to the NuttX Community: Alan Carvalho de Assis, Tomasz Cedro, Xiang Xiao, and Alin Jerpelea,
my fellow GSoC-mate Saurav Pal, and others for their assistance and encouragement during challenging phases of the project. Their feedback and advice significantly contributed to the success of the project.

I would also like to thank my parents, other family members and friends for their support throughout this journey.

Finally, I am grateful to Google, Stephanie and Lucila (GSoC Admins) for organizing the 20th Google Summer of Code and for providing a platform for students like me to learn and contribute to open-source projects.

Thank you once again to everyone who made this experience enriching and unforgettable.
