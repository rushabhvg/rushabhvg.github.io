
Hello! Welcome to my blog about my experience with GSOC 2024 mid terms!



Introduction
I am Rushabh Vipul Gala, studying Computer Science and Engineering at University of Mumbai, India. I love to solve real world challenges, and want to help for the betterment of the world. I have keen interest in new technologies. And, I am thrilled to be able to contribute to the Open Source Community throught Google Summer of Code.

I was curious about the buzz the around the Rust language. Rust is gaining popularity as a memory safe language. I tried writing some code in Rust. It was a bit difficult in the begining, and afterwards I slowly started to grasp it. And, hence started to look around Rust and it's applicaitons.

For Google Summer of Code 2024, I am contributing to the Apache's NuttX on the project "PROJECT_TITLE". The aim of this project is to prepare a foundation for the developers to write NuttX apps in Rust language. This project particularly interested me because, I could understand the NuttX ecosystem, and loved Rust. I am excited to write code in Rust, a memory safe language gaining attention world wide. And contribute to the open source community.

In this blog post, I will share my journey through the mid-term phase of GSoC 2024, highlighting the progress made, challenges encountered, and the invaluable lessons learned along the way. I hope this glimpse into my experience will shed light on the details of the project and also inspire fellow developers and enthusiasts to contribute to Open Source and learn new age technologies.



Project Overview
My project for Google Summer of Code 2024 is titled [Project Title], and I am working in collaboration with The Apache Software Foundation. The main goal of my project is to port the NuttX Apps from C to Rust, write various Rust wrappers for Unsafe C code. This will contribute to help the developers to code and deploy applications in Rust. The project addresses the issues with Rust Unsafe blocks of code and wrapper functions. This is crucial because the traditional C code is vulnerable to memory-based attacks. And, NuttX is a real-time operating system, thus, the saftey is at the core.

By the mid-term evaluation, I aimed to achieve milestones such as having implemented Embedded Rust, C and Rust interoperatibility, presented at NuttX Workshop, port the LED Blinky App from C to Rust, deploy LED Blinky on Ox64 BL808 SBC, add and test GPIO and LED drivers for Ox64 BL808 SBC. These milestones are critical as they mark key progress points towards the overall completion of the project.

The tasks completed for the mid-term evaluations are:
- Implement Embedded Rust
- C Interoperability with Rust (based on Standard Rust)
- Presentation at NuttX Workshop
- C Interoperability with Rust (unsafe open and ioctl)
- Port the LED Blinky App from C to Rust
- Demo Ox64 Emulator at NuttX Workshop
- Flash Ox64 SBC
- Test Rust Blinky on Ox64 Emulator Ox64 SBC
- Add and test the GPIO Driver (in C) for NuttX Kernel on Ox64 Emulator Ox64 RISC-V Single-Board Computer
- Add and test the LED Driver (in C) for NuttX Kernel on Ox64 Emulator Ox64 RISC-V Single-Board Computer

During the first phase of GSoC 2024, I have successfully acheived C and Rust interoperability, and implemented LED Blinky in Rust. This include writing Unsafe wrappers for file and IOCTL commands in Rust, converting the LED Blinky from C to Rust, working with Strings in Rust.



Lessons learnt and Mentorship:

Throughout the development process, I encountered several challenges, one of the major challenges I faced was the Cargo issue. Typically any Rust project uses Cargo for dependency management and builing the files. The NuttX developers emphasise on System Control over everything, and Cargo's automatic dependency handling might not match up with the strict needs of NuttX. To overcome this, we (myself, and my mentor Mr. Lup Yuen Lee) decided to handle eveything manualy, i.e. checking and downloading every dependency, linking these dependencies, compiling, and building them together.

Thanks to all this challeges and hurdles, I was able to enhanced my proficiency in Rust, and C, and programming in general. I have learnt how to download and build the external libraries, compile a Rust application in a real-world situation. I learnt how to document the code, and improved various non-technical skills like, Presentation, Timing myself, Team work, Communication, and how to tackle the issues while coding in collaboration. I also learnt about a interesting concept - Code Ownership. Working closely with my mentor and engaging with the open-source community has significantly improved my ability to communicate technical concepts effectively and collaborate efficiently.

I received a lot of help from my mentor, My Lup Yuen Lee. He is a member of Apache NuttX PMC (Project Management Committee). He was a lecturer before this joining the Apache NuttX PMC. Through his experience as a lecturer, he was helping me a final-year student in various tasks which might be facile for an experienced developer, and I sometiems found it a bit sophisticated. His guidance and advices have helped me a lot. In the begining, I was unable to even compile the NuttX, he made a step-by step guide on how to build and run NuttX, which actually helped me a lot. Once, I was facing some difficulty in flashing the Ox64 BL808 board, he had promptly help me flash it.

The NuttX community is too kind. I was able to solve many of the NuttX-related issues with the help of my mentor, and the community. The developers are friendly to new-comers and help them prompty.



Mid-Term Evaluation Experience:
I conducted rigorous testing of the implemented features to identify and resolve any potential issues. Additionally, I reviewed my codebase to ensure adherence to coding standards and best practices. I have also ran a automatic code style checking tool, nxstyle, to check and resolve any conflicts with coding standards of NuttX.

During the mid-term evaluation, I received positive feedback from my mentor regarding the successful implementation of features and improvements. They appreciated my work and were satishfied with my work and the code I have delivered.

I also received valuable feedback on areas where further optimization and refinement are needed, particulary in my working speed, where my mentor said that I was sometimes progressing too quickly and sometimes I was a bit slower. Overall my speed was good, I just need to pace-up sometimes, and slow-down sometimes. Because of the advice and feedback recieved, we have mututally re-distributed the work/deliverables to match the GSOC timeline.

Moving forward, my primary goal is to create and document the Rust Wrappers. This will help in writing faster and safer NuttX Apps. Also, expand the support for NuttX Apps in Rust to RISC-V 32-bit, RISC-V 64-bit, Arm32 and Arm64 systems. Thus, achieveing our initial goal of preparing a foundation for other developers to develop and code NuttX Apps in Rust. Beyond GSoC, I aim to continue contributing to the NuttX project as an active member of the open-source community. I plan to collaborate with my mentor to develop more NuttX Apps in Rust, and help the other developers worldwide.



Personal Reflections:
Throughout GSoC 2024, I've learned the importance of modular design and clean coding practices. Implementing LED Blinky App taught me more about Rust and C, how do embedded systems work, how to write Rust in C, and C in Rust. I have the learnt the importance of dividng the work in smaller parts and completing them in an orderly manner. I learnt how to divide a huge task into smaller chunks and complete these chunks ste-by-step.

Collaborating with my mentor and engaging with the community has broadened my perspective on teamwork. I've learned to leverage collaborative tools like Git and Discord for effective communication and version control. Personally, GSoC has boosted my confidence in tackling complex technical challenges and handling feedback constructively. It's been a journey of continuous learning and self-improvement.

One of my proudest acheivemnt is LED Blinky app in Rust. I faced many difficulties in handling the file and IOCTL operations in Rust. With my mentor's help, I was able to write Unsafe wrappers for these operations, which in turn helped me write the app. I was having some difficulty handling Strings and printing the strings as a output to console. My findings about the different data types of Strings, Characters, and pointers in Rust and C helped me understand the different prinitng function like, "printf", and "puts".




Some Questions asked by my mentor, Mr Lup Yuen Lee:
(a) We had a very interesting NuttX International Workshop. What do you think about the NuttX Project and the NuttX Community?
 -> The NuttX International Workshop was very interesting and I came to know and learn a lot about the NuttX community. I was excited to communicate and talk with other NuttX Developers around the world. Their research and projects left me surprised. I re-learnt how big and amazing the NuttX project is actually in reality. I loved the NuttX workshop and would love to attend more such workshops in the future.

(b) How was your experience presenting at the NuttX Workshop? Do you think the experience might be helpful for your future career?
-> Honestly, this was the first time I had ever presented anything. I was nervous and excited to present in an international workshop. Through my presentation, I was able to explain the community, how we are going to port NuttX Apps from C to Rust. Considering this was my first presentation, I feel it was a good one. And, after watching my presentation a few more times, I was able to find the some areas of improvement like, the wordings and pace of speaking. This presentation has boosted my self-confidence to give more presentaions.
And, connecting to many experts, has surely helped me progress in my career. Thanks. 

(c) How do you feel about your First Contribution to NuttX Kernel? What were the challenges that you faced?
-> I was feeling a lot nervous while making my first contribution to NuttX Kernel. As, the NuttX Kernel is the core of the NuttX project, I was scared if I would be able to code as per the NuttX standards and be able to contribute. We had the BL808 Courier issue, because of that BL808 courier issue, we weren't able to build the LED Blinky app. I was sad, and a bit stressed. After it was resolved, we were able to build the LED Blinky apps again, and after getting a lot of suggestions from my mentor, I was confident in the code I have written. I was excited to submit my first PR to the NuttX Kernel mainline. I was a lot happy once the pull request got accepted.

(d) Tell us a bit about the Rust Blinky App that you have created for NuttX. What are your impressions of Rust so far?
-> The Rust Blinky App is a simple implementation of LED Blinky App, where the user controls LEDs throught application. And, instead of C, the code was written in Rust for NuttX. The LEDs are turned on or off from the command line. And, as we know Rust is a memory safe language, it sometimes gets quiet pricky to write the code for handling Characters, Strings, and pointers. Anyways, once we handle these data types carefully, Rust is good. It's memory safety and Zero cost abstraction is very helpful while writing performance critical code.

(e) What were the challenges you faced while using the Ox64 SBC? Is there anything that NuttX Project (or PINE64) could do better, to make Ox64 programming easier for learners?
-> I have many challenges while usign the Ox64 SBC. I faced difficulties setting and flashing NuttX on it. Connecting the Ox64 SBC to laptop was also a bit complex task for me. However, I would say that all of these hurdles were just diffcult for me because of my lack of knowledge about these, and once I got the hang of Ox64 SBC, I was able to connect, set-up, and flash NuttX easily on it. I would just say, a bit detailed documentation is good for absoulte begineers like me. And, everything else works fine because of the NuttX Project, and PINE64 continuos support.

(f) How are you using the Ox64 Emulator for GSoC? Do you think Ox64 Emulator is a good substitute if Ox64 SBC is unavailable?
-> I have set-up Ox64 Emulator with the help of temu (a tiny emulator). It perfectly does the work. I find it helpful and useful. Yes, I guess Ox64 Emulator is a good substitue if Ox64 SBC is unavailable. And, we should keep in mind that an emulator is not same the physical hardware. Hence, for the deployment and production, we should thoroughly test the program on both - Emulator and Physical Hardware. As sometimes, the same piece of code might not work on hardware device, even if it works on emulator.

(g) We had some Power Outage problems during GSoC. How did you continue working in spite of the outage?
-> Yeah, I had Power Outage during the starting phase. I was quite surprised because of we have almost Zero outages. It was kind of challenging as the power outages had coincided with week in which I was about to prepare for NuttX workshop. To deal with it, I used to sleep/relax while the power was gone. Or, sometimes stuided more about Rust and Embedded System on my mobile phone. Once, the power was back on, I used to work on my laptop till the battery lasts, and continously save the work, just in case the laptop battery dies and power goes. And thanks to my mentor, Mr. Lup, who helped and cooperated with me, I was able to handle the Power Outages and still be able to contribute to the NuttX Project. 

(h) Is there anything that NuttX Project can help, so new devs can get onboard NuttX quicker?
-> NuttX Project is very big and complex to understand and learn. And, I would just say that, a beginner/starter's guide is good for the new devs who want to onboard NuttX. I think a beginner's guide should just cover the high level structure of the Project, for example, what functionality is inside what, and current major issues and how is it being handled. Anyways, even without this guide, the devs can onboard NuttX project because of the versatile and friendly community.

(i) Would you recommend GSoC and NuttX to your fellow students? 
-> Yes, I would highly recommend my fellow students to join GSOC and NuttX. I promote open-source contribution and help my fellow students learn about conding and programming. I guide to the open-source world through various programs like Google Summer of Code and other such programmes. This GSoC and NuttX project has helped me boost my self-confidence and showcase my developing capabilites to the world.



Acknowledgments:
I would like to thank all everyone who has helped and supported me during the GSoC period.

I am also grateful to Mahadev, Bhagwan Vishnu, and all the gods and goddesses for granting me this opportunity and guiding me through this journey.

I am incredibly grateful to Mr. Lup Yuen Lee for his continuous support, patience, and invaluable guidance throughout the project. His expertise and encouragement were instrumental in shaping my understanding and skills in embedded systems.

A special thank you to The Apache Software Foundation for providing me with this amazing opportunity to participate in GSoC. The resources and community at The Apache Software Foundation were essential in helping me achieve my goals and grow as a developer.

I extend my thanks to Alan Carvalho de Assis, Tomasz CEDRO, Xiang Xiao, Alin Jerpelea, Saurav Pal, and others for their assistance and encouragement during challenging phases of the project. Their feedback and advice significantly contributed to the success of the project.

I would also like to thank my family and friends for their unwavering support and understanding throughout this journey.

Finally, I am grateful to Google, Stephanie and Lucila (GSoC Admins) for organizing 20th Google Summer of Code and providing a platform for students like me to learn and contribute to open-source projects.

Thank you once again to everyone who made this experience enriching and unforgettable.
