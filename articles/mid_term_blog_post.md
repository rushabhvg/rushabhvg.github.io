
Hello! Welcome to my blog about my experience with GSOC 2024 mid terms!



# Introduction

I am Rushabh Vipul Gala, studying Computer Science and Engineering at the University of Mumbai, India. I love to solve real-world challenges, and want to contribute for the betterment of the world. I have a keen interest in new technologies. And I am thrilled to be able to contribute to the Open Source Community through Google Summer of Code (GSoC).

I was curious about the buzz around the Rust language. Rust is gaining popularity as a memory safe language. I tried writing some code in Rust. It was a bit difficult in the beginning, and afterwards I slowly started to grasp it. And hence started to look around Rust and its applications.

For Google Summer of Code 2024, I am contributing to Apache NuttX on the project "Apache NuttX Apps and Rust Integration". The aim of this project is to prepare a foundation for developers to write NuttX apps in the Rust language. This project particularly interested me because I could understand the NuttX ecosystem, and loved Rust. I am excited to write code in Rust, a memory safe language gaining attention worldwide and contribute to the open source community.

In this blog post, I will share my journey through the mid-term phase of GSoC 2024, highlighting the progress made, challenges encountered, and the invaluable lessons learned along the way. I hope this glimpse into my experience will shed light on the details of the project and also inspire fellow developers and enthusiasts to contribute to Open Source and learn new-age technologies.



# Project Overview

My project for Google Summer of Code 2024 is titled "Apache NuttX Apps and Rust Integration," and I am working in collaboration with The Apache Software Foundation. The main goal of my project is to port the NuttX Apps from C to Rust and write various Rust wrappers for Unsafe C code. This will help developers to code and deploy applications in Rust. The project addresses issues with Rust Unsafe blocks of code and wrapper functions. This is crucial because traditional C code is vulnerable to memory-based attacks. Additionally, NuttX is a real-time operating system; thus, safety is critical.

By the mid-term evaluation, I aimed to achieve milestones such as implementing C and Rust interoperability, presenting at the NuttX Workshop, porting the LED Blinky App from C to Rust, deploying LED Blinky on Ox64 BL808 SBC, and adding GPIO and LED drivers for Ox64 BL808 SBC. These milestones are critical as they mark key progress points towards the overall completion of the project.

The tasks completed for the mid-term evaluations are:

- Implemented Embedded Rust
- C Interoperability with Embedded Rust (no_std file I/O and ioctl)
- Ported the LED Blinky App from C to Rust
- Tested Rust Blinky on Ox64 Emulator
- Presented at NuttX Workshop
- Demonstrated Ox64 Emulator at NuttX Workshop
- Flashed Ox64 SBC
- Upstreamed the GPIO Driver (in C) to NuttX Kernel for Ox64 SBC
- Upstreamed the LED Driver (in C) to NuttX Kernel for Ox64 SBC

During the first phase of GSoC 2024, I successfully achieved C and Rust interoperability and implemented LED Blinky in Rust. This includes implementing file and IOCTL commands in Rust and converting the LED Blinky App from C to Rust.



# Lessons Learnt and Mentorship

Throughout the development process, I encountered several challenges. One of the major challenges I faced was the Cargo issue. Typically, any Rust project uses Cargo for dependency management and building files. NuttX developers require careful system control, and Cargo's automatic dependency handling might not align with the strict needs of NuttX. To overcome this, my mentor, Mr. Lup Yuen Lee, and I decided to handle everything manually: checking and downloading every dependency, linking these dependencies, compiling, and building them together.

Thanks to all these challenges and hurdles, I was able to enhance my proficiency in Rust, C, and programming in general. I learned how to download and build external libraries and compile a Rust application in a real-world situation. I also learned how to document code and improved various non-technical skills such as presentation, pacing, teamwork, communication, and how to tackle issues while coding in collaboration. Additionally, I learned about an interesting concept - Code Ownership. Working closely with my mentor and engaging with the open-source community has significantly improved my ability to communicate technical concepts effectively and collaborate efficiently.

I received a lot of help from my mentor, Mr. Lup Yuen Lee, who is a member of Apache NuttX PMC (Project Management Committee). He was a lecturer before joining the Apache NuttX PMC. Through his experience as a lecturer, he has assisted me (as a final-year student) with various tasks that might be facile for an experienced developer but were sometimes challenging for me. His guidance and advice have been invaluable. Initially, I struggled even to compile NuttX, but his step-by-step guide on how to build and run NuttX was tremendously helpful. On another occasion, when I encountered difficulty flashing the Ox64 BL808 board, he promptly provided assistance.

The NuttX community is incredibly supportive. With the help of my mentor and the community, I was able to resolve many NuttX-related issues. The developers are welcoming to newcomers and provide prompt assistance.



# Mid-Term Evaluation Experience

I conducted rigorous testing of the implemented features to identify and resolve any potential issues. Additionally, I reviewed my codebase to ensure adherence to coding standards and best practices. I also ran an automatic code style checking tool, nxstyle, to identify and resolve any conflicts with NuttX coding standards.

During the mid-term evaluation, I received positive feedback from my mentor regarding the successful implementation of features and improvements. He appreciated my work and was satisfied with the code I delivered.

I also received valuable feedback on areas needing further optimization and refinement, particularly regarding my work pace. My mentor noted that sometimes I progressed too quickly and at other times I was a bit slower. Overall, my speed was good; I just need to speed up sometimes and slow down others. Based on this advice and feedback, we have mutually adjusted our work and deliverables to better align with the GSoC timeline.

Moving forward, my primary goal is to create and document Rust wrappers. This will facilitate faster and safer development of NuttX Apps in Rust. Additionally, I aim to expand support for NuttX Apps in Rust to include RISC-V 32-bit, RISC-V 64-bit, Arm32, and Arm64 systems. This aligns with our initial goal of establishing a foundation for developers to write NuttX Apps in Rust. Beyond GSoC, I intend to continue contributing to the NuttX project as an active member of the open-source community. I plan to collaborate with my mentor to develop more NuttX Apps in Rust and assist developers worldwide.



# Personal Reflections

Throughout GSoC 2024, I've learned the importance of modular design and clean coding practices. Implementing the LED Blinky App taught me more about Rust and C, how embedded systems work, how to call Rust from C, and C from Rust. I have learned the importance of dividing the work into smaller parts and completing it in an orderly manner, step by step.

Collaborating with my mentor and engaging with the community has broadened my perspective on teamwork. I've learned to leverage collaborative tools like Git and Discord for effective communication and version control. Personally, GSoC has boosted my confidence in tackling complex technical challenges and handling feedback constructively. It's been a journey of continuous learning and self-improvement.

One of my proudest achievements is the LED Blinky App in Rust. I faced many difficulties in handling file I/O and IOCTL operations in Rust. With my mentor's help, I was able to implement these operations, which in turn helped me write the app. I also encountered challenges with handling strings and printing them to the console. My exploration of different data types for strings, characters, and pointers in Rust and C helped me understand the various approaches to calling console output functions.




Some questions asked by my mentor, Mr Lup Yuen Lee:

_(a) We had a very interesting NuttX International Workshop. What do you think about the NuttX Project and the NuttX Community?_

The NuttX International Workshop was indeed interesting, and I learned a lot about the NuttX Community. I was excited to communicate and talk with other NuttX developers around the world. Their research and projects left me surprised. I re-learned how big and amazing the NuttX project actually is. I loved the NuttX workshop and would love to attend more such workshops in the future.

_(b) How was your experience presenting at the NuttX Workshop? Do you think the experience might be helpful for your future career?_

Honestly, this was the first time I had ever presented anything. I was nervous and excited to present at an international workshop. Through my presentation, I explained the community and our plans to port NuttX Apps from C to Rust. Considering this was my first presentation, I feel it went well. After reviewing my presentation a few times, I identified areas for improvement, such as wording and pace of delivery. This experience has boosted my self-confidence for future presentations. Connecting with many experts has also helped me progress in my career. Thanks.

_(c) How do you feel about your First Contribution to NuttX Kernel? What were the challenges that you faced?_

I was very nervous while making my first contribution to the NuttX Kernel. As the NuttX Kernel is the core of the NuttX project, I was worried about coding according to NuttX standards and being able to contribute effectively. We encountered an issue with another BL808 Driver, which prevented us from building the LED Blinky app. I felt disappointed and stressed during that time. After resolving the issue, we successfully built the LED Blinky app again. With guidance from my mentor and receiving many suggestions, I gained confidence in the code I had written. I was excited to submit my first PR to the NuttX Kernel mainline, and I was thrilled once the pull request got merged.

_(d) Tell us a bit about the Rust Blinky App that you have created for NuttX. What are your impressions of Rust so far?_

The Rust Blinky App is a simple implementation of the LED Blinky App, where the user controls an LED through the application. Instead of using C, the code was written in Rust for NuttX. The LED can be turned on or off from the command line. Rust, being a memory-safe language, can sometimes be tricky when handling characters, strings, and pointers. However, with careful management of these data types, Rust proves to be effective. Its memory safety and zero-cost abstraction are particularly advantageous when writing performance-critical code.

_(e) What were the challenges you faced while using the Ox64 SBC? Is there anything that NuttX Project (or PINE64) could do better, to make Ox64 programming easier for learners?_

I encountered several challenges while using the Ox64 SBC. Setting up and flashing NuttX on it posed difficulties for me. Connecting the Ox64 SBC to my laptop was also somewhat complex. However, I attribute these challenges mainly to my lack of initial knowledge. Once I became familiar with the Ox64 SBC, I found it easier to connect, set up, and flash NuttX. I believe that more detailed documentation would greatly benefit absolute beginners like me. Nonetheless, everything functioned well due to the support from the NuttX Project and PINE64.

_(f) How are you using the Ox64 Emulator for GSoC? Do you think Ox64 Emulator is a good substitute if Ox64 SBC is unavailable?_

I have configured the Ox64 Emulator with the help of TEMU (the tiny emulator), and it has proven to be effective for my work. While the Ox64 Emulator serves as a reliable substitute when the Ox64 SBC is unavailable, it's important to note that an emulator does not replicate physical hardware precisely. Therefore, it is crucial to thoroughly test programs on both the emulator and physical hardware for deployment and production. Occasionally, code that functions correctly on the emulator may behave differently on the actual hardware.

_(g) We had some Power Outage problems during GSoC. How did you continue working in spite of the outage?_

Yeah, I had a power outage during the starting phase. I was quite surprised because we have almost zero outages. It was challenging as the power outages coincided with my preparation for the NuttX Workshop. To deal with it, I used to sleep/relax while the power was gone. Sometimes I studied more about Rust and Embedded Systems on my mobile phone. Once the power was back on, I used to work on my laptop as long as the battery lasts, continuously saving the work, just in case the laptop battery dies and the power goes out. And thanks to my mentor, Mr. Lee, who helped and coordinated with me, I was able to handle the power outages and still contribute to the NuttX Project. 

_(h) Is there anything that NuttX Project can help, so new devs can get onboard NuttX quicker?_

NuttX Project is very big and complex to understand and learn. And, I would just say that a beginner's guide is good for the new devs who want to get onboard with NuttX. I think a beginner's guide should just cover the high-level structure of the project, for example, which functionality is inside where, the current issues, and how they are handled. Even without this guide, the devs can get onboard with the NuttX Project because of the versatile and friendly community.

_(i) Would you recommend GSoC and NuttX to your fellow students?_ 

Yes, I would highly recommend my fellow students to join GSoC and NuttX. I am keen to promote open-source contribution, helping my fellow students learn about coding and programming. I will guide them towards the open-source world through various programs like Google Summer of Code and other such programs. GSoC and the NuttX Project have helped boost my self-confidence, showcasing my coding capabilities to the world.



# Acknowledgments

I am also thankful to Mahadev, Bhagwan Vishnu, and all the gods and goddesses for granting me this opportunity and guiding me through this journey.

I am incredibly grateful to Mr. Lup Yuen Lee for his continuous support, patience, and invaluable guidance throughout the project. His expertise and encouragement were instrumental in shaping my understanding and skills in embedded systems.

A special thank you goes to the Apache Software Foundation for providing me with this amazing opportunity to participate in GSoC. The resources and community at the Apache Software Foundation were essential in helping me achieve my goals and grow as a developer.

I am also grateful to PINE64 for sponsoring me with two Ox64 Single Board Computers featuring the Bouffalo Lab BL808 RISC-V SoC, along with their associated setup tools. These resources were essential for testing my code and applications on physical hardware.

I extend my thanks to Alan Carvalho de Assis, Tomasz Cedro, Xiang Xiao, Alin Jerpelea, Saurav Pal, and others for their assistance and encouragement during challenging phases of the project. Their feedback and advice significantly contributed to the success of the project.

I would also like to thank my parents, other family members and friends for their unwavering support and understanding throughout this journey.

Finally, I am grateful to Google, Stephanie and Lucila (GSoC Admins) for organizing the 20th Google Summer of Code and for providing a platform for students like me to learn and contribute to open-source projects.

Thank you once again to everyone who made this experience enriching and unforgettable.
