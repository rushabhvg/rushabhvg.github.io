
Hello! Welcome to my blog about my experience with GSOC 2024 mid terms!

# Introduction
I am Rushabh Vipul Gala, pursuing a degree in Computer Science and Engineering at the University of Mumbai, India. My passion lies in tackling real-world challenges and leveraging technology for a positive impact on the world. I have a keen interest in exploring emerging technologies and am honored to be making a meaningful contribution to the Open Source Community through Google Summer of Code (GSoC).

My journey into the realm of Rust programming language began with a curiosity sparked by growing popularity of Rust as a memory-safe language. Despite facing initial difficulties, I gradually immersed myself in Rust, understanding its nuances and exploring its diverse applications. This exploration led me to focus on contributing to Apache NuttX for GSoC 2024, working on the project "Apache NuttX Apps and Rust Integration".

The core objective of this project is to establish a foundation for developers to create NuttX applications using the Rust programming language. The synergy between the NuttX ecosystem and my interests for Rust prompted my involvement in this endeavor. Embracing Rust, a globally recognized memory-safe language, excites me as I engage in being a part of the open-source community.

In this blog post, I aim to provide insights into my progress during the mid-term phase of GSoC 2024. I will share the milestones achieved, challenges faced, and valuable insights gained along this rewarding journey. My hope is that this narrative will offer a glimpse into the intricate details of the project, inspiring fellow developers and technology enthusiasts to engage with open source initiatives and embrace cutting-edge technologies.

# Project Overview
My project for Google Summer of Code 2024, in partnership with The Apache Software Foundation, is focused on "Apache NuttX Apps and Rust Integration". The primary objective of the project is to transition some basic NuttX Apps from C to Rust, develop Rust wrapper blocks for Unsafe C code, and provide developers with the tools to code and deploy applications using Rust. This initiative addresses concerns related to Rust Unsafe code blocks and wrapper functions, which are pivotal in enhancing security given the susceptibility of traditional C code to memory-based attacks. And, as NuttX functions as a real-time operating system, prioritizing safety is imperative.

By the mid-term evaluation mark, I had aimed to achieve significant milestones, which included establishing C and Rust interoperability, presenting at the NuttX Workshop, migrating the LED Blinky App from C to Rust, deploying LED Blinky on the Ox64 BL808 Single-Board Computer (SBC), and integrating GPIO and LED drivers for the Ox64 BL808 SBC. These milestones signify critical progress points contributing to the overall project completion.

Key tasks completed for the mid-term evaluation phase are as follows:
- Implementation Embedded Rust
- C Interoperability with Embedded Rust (incorporating no_std file I/O and ioctl)
- Migration of the LED Blinky App from C to Rust
- Testing Rust Blinky on the Ox64 Emulator
- Delivering a presentation at the NuttX Workshop
- Demonstrating the Ox64 SBC & Ox64 Emulator at the NuttX Workshop
- Flashing the Ox64 SBC
- Upstreaming the GPIO Driver (in C) to the NuttX Kernel for the Ox64 SBC
- Introducing the LED Driver (in C) to the NuttX Kernel for the Ox64 SBC

During the initial phase of GSoC 2024, I have successfully achieved C and Rust interoperability, along with implementing the LED Blinky functionality in Rust. This involved incorporating file and IOCTL commands in Rust and transitioning the LED Blinky App from C to Rust, marking significant progress.

# Lessons Learnt and Mentorship
During the development process, I had encountered various challenges, with one of the major obstacle being related to the usage of Cargo, the standard dependency management and building tool for Rust projects. In the case of NuttX development, the precise control required by the NuttX system did not align well with Cargo's automatic dependency handling. To address this, my mentor, Mr. Lup Yuen Lee, and I made the decision to manually handle all dependencies by checking and downloading each one of them, linking them, and compiling and building them together.

These challenges and hurdles provided valuable learning opportunities, allowing me to significantly improve my proficiency in Rust, C, and programming in general. I have gained experience in downloading and building external libraries and compiling a Rust application in a real-world scenario. Additionally, I have learnt the importance of proper code documentation and enhanced various non-technical skills, such as presentation skills, task scheduling, teamwork, communication, and problem-solving in a collaborative coding environment. I have also discovered the concept of code ownership, as working closely with my mentor and engaging with the open-source community improved my ability to effectively communicate technical concepts and collaborate efficiently.

I am deeply grateful for the tremendous support and guidance provided by my mentor, Mr. Lup Yuen Lee, who is a member of the Apache NuttX PMC (Project Management Committee) and formerly a lecturer. His prior experience as a lecturer allowed him to assist me, as a final-year student, with various tasks that may have seemed straightforward for an experienced developer but proved to be more challenging for me. He created a step-by-step guide on how to build and run NuttX when I was initially unable to even compile it. Additionally, when I encountered difficulties in flashing the Ox64 BL808 board, he promptly provided assistance.

The NuttX community has also been incredibly supportive. With the help of my mentor and other community members, I was able to resolve many NuttX-related issues. The developers within the community are welcoming to newcomers and offer prompt assistance.

Overall, this mentorship experience and collaboration with the NuttX community have been tremendously beneficial, providing me with valuable skills, knowledge, and the support needed to overcome challenges and successfully contribute to the project.

# Mid-Term Experience
I have conducted testing of the said implemented features to detect and resolve any potential issues. Furthermore, I have performed a thorough review of my codebase, ensuring strict compliance with coding standards and the best practices. Additionally, I have utilized nxstyle, an automatic code style checking tool, to identify and rectify any deviations from coding standards set by NuttX.

During the mid-term evaluation, I have received constructive feedback from my mentor regarding the successful implementation of features and improvements. He has acknowledged my efforts and expressed satisfaction with the code that I have delivered. I had received invaluable feedback on areas that require optimization and refinement, particularly in terms of my working speed. While my mentor praised my work pace, he suggested that I occasionally need to increase or decrease my speed depending on the task at hand. Based on this feedback, we have mutually reallocated work to match the GSOC timeline.

Moving forward, I have prioritize developing and documenting the Rust wrapper blocks to accelerate the development of faster and safer NuttX Apps. Additionally, I have aim to expand NuttX support in Rust to include RISC-V 32-bit, RISC-V 64-bit, Arm32, and Arm64 systems. This will lay the groundwork for other developers to code NuttX Apps in Rust. Beyond the scope of GSoC, I endeavor to continue contributing to the NuttX project as an active member of the open-source community. I plan to work alongside my mentor to create more NuttX Apps in Rust and aid developers worldwide.

# Personal Reflections
Throughout the Google Summer of Code 2024 (GSoC 2024), I have gained valuable insights into the significance of modular design and maintaining clean coding practices. My experience in developing the LED Blinky App has deepened my understanding of the Rust and C programming languages, embedded systems functionality, and the intricacies of interfacing Rust with C and vice versa. I have also grasped the importance of breaking down tasks into manageable components and executing them methodically, step by step.

Collaborating closely with my mentor and actively participating in the community has significantly broadened my perspective on effective teamwork. I have become proficient in utilizing collaborative tools such as Git and Discord for streamlined communication and version control. Personally, GSoC has bolstered my confidence in tackling intricate technical challenges and embracing constructive feedback, fostering a continuous journey of learning and self-improvement.

Among my most notable achievements during this period is the successful development of the LED Blinky App using Rust. Overcoming challenges, particularly in managing File I/O and IOCTL operations within Rust, was a significant learning curve. With invaluable guidance from my mentor, I successfully implemented these operations, which were pivotal in the app's development. I encountered specific difficulties in handling strings and their output to the console. Through diligent research, I gained insights into Rust's and C's distinct data types for strings, characters, and pointers, enhancing my ability to effectively utilize console output functions.

Some questions asked by my mentor, Mr Lup Yuen Lee:

_(a) We had a very interesting NuttX International Workshop. What do you think about the NuttX Project and the NuttX Community?_

The NuttX International Workshop was indeed captivating, providing me with a profound understanding of the NuttX Project and its vibrant community. Engaging with NuttX developers globally was both enlightening and inspiring. I was particularly impressed by the diverse research initiatives and projects showcased during the workshop. This experience reaffirmed my appreciation for the breadth and significance of the NuttX project. I thoroughly enjoyed the workshop and eagerly anticipate participating in future events to further enrich my knowledge and contribute to this remarkable community.

_(b) How was your experience presenting at the NuttX Workshop? Do you think the experience might be helpful for your future career?_

Presenting at the NuttX Workshop was a significant milestone for me, as it marked my inaugural experience in public speaking. Naturally, I approached it with a mix of nervousness and excitement, given the international audience. During my presentation, I effectively conveyed insights into our initiative to migrate NuttX Apps from C to Rust, which was well-received by attendees.

Reflecting on this experience, I believe my presentation was a solid debut effort. Upon reviewing recordings, I identified areas for improvement in terms of clarity in wording and pacing of delivery, which I'm eager to refine for future engagements. This opportunity has notably bolstered my confidence in public speaking and underscored the value of connecting with industry experts, which I believe will positively influence my career trajectory.

Overall, presenting at the NuttX Workshop was not only a valuable learning experience but also a pivotal step in my professional development.

_(c) How do you feel about your First Contribution to NuttX Kernel? What were the challenges that you faced?_

I approached my first contribution to the NuttX Kernel with a mixture of excitement and nervousness. The NuttX Kernel forms the cornerstone of the entire NuttX project, so ensuring my code met its rigorous standards was paramount. Initially, I faced challenges related to a BL808 Driver issue, which temporarily halted progress on the LED Blinky app development. This setback was disappointing and created some stress.

Fortunately, with guidance and feedback from my mentor, I navigated through these obstacles and resolved the issue. This experience not only strengthened my coding skills but also instilled confidence in my ability to contribute effectively. Submitting my first pull request to the NuttX Kernel was a moment of great satisfaction and validation. Witnessing its successful merge was a testament to my growth and dedication to the project.

Overall, while the journey had its share of challenges, overcoming them and seeing tangible results has been immensely rewarding and motivating for me.

_(d) Tell us a bit about the Rust Blinky App that you have created for NuttX. What are your impressions of Rust so far?_

The Rust Blinky App I developed for NuttX is a straightforward application that allows users to control an LED via command-line inputs. Unlike traditional implementations in C, this app leverages Rust's capabilities within the NuttX environment. Users can toggle the LED on or off, demonstrating basic functionality using Rust's syntax and features.

My experience with Rust has been positive overall. Rust's focus on memory safety is particularly noteworthy, although it does introduce complexities when handling data types such as characters, strings, and pointers. However, these challenges are outweighed by Rust's benefits, especially its zero-cost abstractions and suitability for writing efficient, performance-critical code.

In summary, Rust has proven to be a valuable tool for developing embedded applications like the Blinky App, offering a robust framework within NuttX while ensuring reliability and performance.

_(e) What were the challenges you faced while using the Ox64 SBC? Is there anything that NuttX Project (or PINE64) could do better, to make Ox64 programming easier for learners?_

Using the Ox64 SBC presented several challenges initially. I encountered difficulties in setting up and flashing NuttX on the device, as well as in establishing a connection between the Ox64 SBC and my laptop. These tasks posed complexities that stemmed largely from my limited experience with the hardware. However, with perseverance and learning, I eventually gained proficiency in these areas, enabling smoother operation of the Ox64 SBC.

To enhance the experience for beginners like myself, I believe more comprehensive documentation would be beneficial. Clearer step-by-step guides and troubleshooting tips specific to the Ox64 SBC would greatly assist newcomers in overcoming initial setup hurdles more efficiently.

_(f) How are you using the Ox64 Emulator for GSoC? Do you think Ox64 Emulator is a good substitute if Ox64 SBC is unavailable?_

In my GSoC project, I've utilized the Ox64 Emulator alongside TEMU, which has proven to be a reliable tool for simulating the Ox64 environment. This emulator effectively mirrors the functionalities of the physical Ox64 SBC, allowing me to test and develop NuttX applications without needing access to the actual hardware.

While the Ox64 Emulator serves as a commendable substitute when physical access to the SBC is unavailable, it's crucial to acknowledge that emulation differs from real-world deployment. Therefore, rigorous testing on both the emulator and the physical Ox64 SBC remains essential. Variations in hardware behavior can occasionally lead to discrepancies, where code that functions correctly in emulation may encounter issues on the actual device.

In summary, leveraging the Ox64 Emulator has facilitated significant progress in my project, providing a practical workaround for development and testing. However, validating applications on physical hardware remains indispensable for ensuring robust performance in real-world scenarios.

_(g) We had some Power Outage problems during GSoC. How did you continue working in spite of the outage?_

Dealing with power outages during the initial phase of GSoC posed unexpected challenges, particularly during critical preparation for the NuttX Workshop. To manage these interruptions, I adopted a proactive approach. During downtime, I utilized the opportunity to rest and recharge, occasionally using my mobile phone to study Rust and embedded systems. Once power was restored, I maximized laptop usage, ensuring continuous progress by diligently saving my work to preempt potential battery drain. Throughout this period, the support and coordination from my mentor, Mr. Lee, were instrumental in navigating these challenges and maintaining productivity on the NuttX Project.

_(h) Is there anything that NuttX Project can help, so new devs can get onboard NuttX quicker?_

The NuttX Project, while rich with opportunities, can present a steep learning curve for newcomers due to its complexity. To facilitate a smoother onboarding process, I recommend enhancing beginner resources. A structured beginner's guide outlining the project's high-level structure, core functionalities, and common issue resolutions would significantly benefit new developers. Clear documentation and accessible learning materials would empower aspiring contributors to engage more effectively with the NuttX community and accelerate their learning curve.

_(i) Would you recommend GSoC and NuttX to your fellow students?_ 

Absolutely, I enthusiastically endorse GSoC and participation in the NuttX Project to my peers and fellow students. These initiatives not only provide invaluable hands-on experience in open-source development but also foster personal growth and skill enhancement in coding and programming. I am committed to encouraging others to explore these opportunities, guiding them towards impactful contributions in the open-source community while showcasing their talents on a global stage.

# Acknowledgments

I am deeply thankful to Mahadev, Bhagwan Vishnu, and all the gods and goddesses for blessing me with this opportunity and guiding me through this transformative experience.

A special appreciation goes to Mr. Lup Yuen Lee for his unwavering support, patience, and invaluable guidance throughout the project. His expertise in embedded systems has been instrumental in shaping my skills and understanding.

I am immensely grateful to the Apache Software Foundation for providing me with the opportunity to participate in GSoC. The resources and supportive community at Apache were indispensable in achieving my goals and personal growth as a developer.

I am grateful to PINE64 for sponsoring me with 2 Ox64 Single Board Computers featuring the Bouffalo Lab BL808 RISC-V SoC, along with their associated setup tools. These resources were instrumental in testing my code and applications on physical hardware, significantly enhancing my development experience.

I extend my sincere thanks to Alan Carvalho de Assis, Tomasz Cedro, Xiang Xiao, Alin Jerpelea, Saurav Pal, and others for their assistance and encouragement during challenging phases of the project. Their feedback and advice were crucial to the project's success.

My heartfelt appreciation also goes to my family and friends for their unwavering support and understanding throughout this journey.

Finally, I would like to express my gratitude to Google, Stephanie and Lucila (GSoC Admins) for organizing the 20th Google Summer of Code and for providing a platform that enabled students like myself to learn and contribute to open-source projects.

Thank you once again to everyone who has made this experience enriching and unforgettable.