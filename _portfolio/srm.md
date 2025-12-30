---
title: "SpaceCraft VR: Space Robotics Manipulators"
excerpt: "Designing Control Inputs for Canadarm2 Simulation"
collection: portfolio
---

title: "Abstract:"
Space Robotics Manipulators is a team focused on the research and development of robotic control algorithms for Space Teams PRO (STP). Specifically, we aimed to implement inverse kinematics within STP, with the aim of allowing users to control a robot arm to achieve a desired end effector pose and velocity. This semester, we focused on simulating Canadarm2, a 7 degree-of-freedom (DOF) robot arm on the ISS used to assist in assembly, maintenance, and visiting vehicle capture. Particularly, my work was on human robot interactions, where I design how a person on a flatscreen or VR will control the Canadarm2 simulation. 

title: "Overall Project Goals:"
* Support a keyboard/mouse, physical joysticks and/or VR hand controllers for human robotic interactions
* Enhance my knowledge in Python programming to work with the simulation
* Educate myself more about various space robotics manipulators and how they function

Accomplishments:
* Was able to create code for controlling one single joint for Canadarm2

What I Wish I Accomplished:
* Creating code for controlling multiple joints at once
* Being able to implement Space Dynamics Subteam’s inverse kinematics algorithms, which is still a work in progress and has not been completed for me to implement into STP
* Implement self-collision in the robotic arm so that it does not bump into any other systems
* Using Virtual Reality to implement the hand controller inputs for a more VR and interactive experience with Canadarm2

Summary of Work:
At the beginning of the semester, I have been doing literature research since the semester started and gained some valuable knowledge by reading Chapter 11 of *Human Spaceflight Operations - Space Robotics* by Megan Levins and Dr. Srinivas Rao Vadali. In particular, I researched more about the four different types of reference frames: frame of resolution, display frame, command frame, hand controller frame. A reference frame in space robotics is also known as a coordinate system and is a fundamental concept that describes the position, orientation and motion of a robots’ rigid bodies or components. I was particularly interested in this since these frames are vital for humans to reference when using these space robotics manipulator systems (SSRMS). Most importantly, the hand controller frame is the essential frame to use toward my design goal since this frame is particularly fixed with respect to workstation hand controllers and map mechanical inputs by operators to command frame and motion on the arm.

After this literary review, I started looking into reading keyboard and controller inputs with Python scripts in order to have an object on the SpaceTeams system move based on the inputs (Pynput library).

After this,  I configured SpaceTeams with Visual Studio. There is currently a program called ArmRunner which controls user inputs with hand controller outputs on SpaceTeams. With this code, I modified it with a version using the Pynput library. This library helps a user press a button (up, down, left, right, etc) and then actually define what that button exactly does. This automatically connects with SpaceTeams and allows the user to use the Canadarm2 through the SpaceTeams simulation. 

After this, I conducted a literary research on self-collision in robotic arms. Some factors I discovered impacting how space robotics manipulators maintain a sense of spatial self-awareness and avoid destructive self-construction are: geometric modeling, constraint motion planning, and real-time barrier and velocity control and constraints. 

The Big Picture & Reflection:
My overall work on controlling hand controller inputs onto the SpaceTeam simulation depended on the work of the Space Dynamics Subteam. They are in charge of what they want to control on the simulation and the robotic manipulator arm, and my work is to implement and define their controls and actions onto the simulation. 
Over the course of this research, I gained a much deeper understanding of how human-robot interactions are designed and implemented within a space robotics environment. I learned how reference frames define the way operators communicate motion to a robotic arm, and how essential these frames are for creating an intuitive control experience. My work with Python, the Pynput library, and the existing ArmRunner code gave me hands-on experience in reading user inputs and translating them into joint motion within the Space Teams PRO simulation. Even though I only achieved single-joint control this semester, this process helped me build foundational skills in programming, debugging, and interfacing with a simulation system.
Researching topics such as inverse kinematics and self-collision also broadened my understanding of the challenges faced by real robotic manipulators like Canadarm2. Although I wasn’t able to implement multi-joint control, VR integration, or collision avoidance yet, studying these areas helped me recognize what is required for safe, realistic robotic motion and where the next steps for this project will be.
Overall, the project was productive and informative. I strengthened my technical skills, learned how different subteams depend on one another, and gained a clearer idea of how complex space robotic systems are designed. This experience prepared me to continue contributing to the team with a better understanding of both the software and the robotics concepts needed moving forward. 


