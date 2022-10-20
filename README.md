# Project 03: Robot Manipulation or Mapping

## Table of Contents

- [Timeline](#timeline)
- [Class Community Guidelines](#class-community-guidelines)
- [Introduction](#introduction)
- [Robot and Team Selection](#robot-and-team-selection)
- [Instructions](#Instructions)

  - [Turtlebot4 Lite](turtlebot4-lite)
  - [EvoArm](#evoarm)

- [Project Demonstration](#project-demonstration)
- [Assessment](#assessment)
- [Receiving Assistance](receiving-assistance)

## Timeline

Activity                   | Deadline
-------------------------- | -------------------------------
Project Work in class:     | November 1st, 2022 during class
Demo and Final Submission: | November 3rd, 2022 by 4:20pm

## Class Community Guidelines

Throughout the completion of this project you must adhere to the [community guidelines](https://github.com/CMPSC-311-Allegheny-College-Fall-2022/course-information/blob/main/community_guidelines.md) that we developed as a class. To report any violations of the code of conduct, please submit an [anonymous form](https://forms.gle/tePfnLY12hyN1Xbd6). Students who think that the class should revise some aspect of the guidelines must use the GitHub issue tracker for that repository to suggest, discuss, and implement any required changes.

By working on and completing this assignment you agree to use the hardware given to you in a responsible manner. Each team is responsible for the safety and security of the robot while it is in your possession. You are allowed to take the robots used in this project outside of ALIC but you have to return all parts at the completion of this project, or if requested, at the end of the semester.

## Introduction

This project assignment invites you to work in a team to implement either an autonomous manipulation or autonomous mapping technique depending on a selected robot type. In this and the next project, the class members will be split into two categories: 1) those working with Turtlebot 4 Lite, and 2) those working with EvoArm. In both cases you will first complete the needed builds and installations to set up and configure a new robotic system. Then, if you are working with EvoArm, you will focus on developing a simple manipulation technique. On the other hand, if you are working with Turtlebot 4 Lite, you will create autonomous mapping for a navigation task. Finally, teams will reflect on their experiences and educate the other teams as they prepare to swap robotic platforms and develop a more advanced application for project 4\. Teams are also responsible for writing a detailed report, stored in the file `writing/report.md`. This is a Markdown file that must adhere to the standards described in the [Markdown Syntax Guide](https://guides.github.com/features/mastering-markdown/).

## Robot and Team Selection

Every member of the course is invited to indicate the preference of the robotic system they will use in this project by completing the [Project 3 Robot Selection form](https://forms.gle/VVhCd5f7HeKN1Mwy5). Class members are also invited to form teams on their own. Instructor will verify everyone's preferences and make final team and robot assignments on October 20th. The teams and the specific robots to be used by them will be noted in the [CMPSC 311 Project Teams spreadsheet](https://docs.google.com/spreadsheets/d/1167k-1ZGXR8TJqWdfp61kC7IDzhSVTUTHP7-Urx7ehc/edit?usp=sharing).

## Instructions

### Turtlebot 4 Lite

You can learn about the hardware specifications of this robot in the [turtlebot4-hardware GitHub repository](https://github.com/turtlebot/turtlebot4-hardware). Please also review the features of this robot on [its website](https://turtlebot.github.io/turtlebot4-user-manual/overview/features.html).

You should first get connected and try to drive the robot using remote control. Please follow [TurtleBot 4 | Unboxing & Getting Started Video](https://www.youtube.com/watch?v=QN01AXjoLdQ&t=0s) to complete this task. Please note that Turtlebot 4 does not inclide Bluetooth Controller but you can drive it using the keyboard buttons as described in the [Driving your Turtlebot 4 Tutorial](https://turtlebot.github.io/turtlebot4-user-manual/tutorials/driving.html).

Please read [Turtlebot 4 Software information](https://turtlebot.github.io/turtlebot4-user-manual/software/) to learn about Turtlebot 4 packages, sensors, using `rviz2`, using SLAM technique to create maps, using navigation stack in ROS 2, and setting up Turtlebot 4 simulator.

Once the robot is up and running, you need to have it generate a map and navigate in the environment. You can follow [Generating a map tutorial](https://turtlebot.github.io/turtlebot4-user-manual/tutorials/generate_map.html) and [Navigation tutorial](https://turtlebot.github.io/turtlebot4-user-manual/tutorials/navigation.html). You can also follow [TurtleBot 4 | Mapping & Navigation with ROS 2 Navigation Stack Video](https://www.youtube.com/watch?v=T3if0aPj0Eo) to learn how to have the Turtlebot build a map and navigate in the environment given the map.

Finally, you need to come up with a navigation task and have your robot build a map of a relatively complex environment and have it navigate for a specific purpose. Instructor approval must be obtained to ensure the select navigation task is appropriate. The source code must be included in the `src/` folder of your project repository. The report must include clear details and experiences from the set up and implementation stages of your project.

Questions and issue logging support can be found at [Turtlebot 4 GitHub Issues](https://github.com/turtlebot/turtlebot4/issues) and [Turtlebot 4 Simulator GitHub Issues](https://github.com/turtlebot/turtlebot4_simulator/issues).

### EvoArm

You can learn more about this robot, what is included in the robotic kit, and the contact information for support by visiting [evodyneacademy's website](https://www.evodyneacademy.com/evoarm-robotic-arm-kit-arduino). Additionally, [EvoArm Flyer](evoarm-kit-insert.pdf) has some helpful information.

This robot has to be built first. Please follow [evodyneacademy tutorials](https://www.evodyneacademy.com/tutorials) to complete all 16 steps of the build process. You will need to use password: `bRtaos40sNd` to access the tutorials. The build process will take about 1 hour.

The provided kit should include micro-sd card that goes into the Raspberry Pi. It already has pre-installed versions of OpenCV and ROS melodic. Once you make the connections between the raspberry pi and the arduino, and connect to the wifi hotspot created by the raspberry pi, the web-interface will start working to control the arm. There are a lot of steps, it will be more clear once you start following the videos. You can then ssh into the raspberry pi and explore around as needed.

Once the robot is up and running, you will need to select an autonomous robotic hand manipulation technique to implement for some application. Keep it simple! Feel free to utilize resources provided in the kit. To find ideas you can also go to [evoarm-apps](https://www.evodyneacademy.com/forum/evoarm-apps), create an account, after after you are approved, you will find lots of information from the community, including sample code and information on how to use ROS and HTTP commands to control/program the arm.

The source code must be included in the `src/` folder of your project repository. The report must include clear details and experiences from the building and implementation stages of your project.

## Project Demonstrations

At the beginning of the lab session on Thursday, October 13th, each team will be given an opportunity to demonstrate their project. When the lab session starts, teams will be given a few minutes to set up their demonstrations and get them running. Then, class members will participate in an interactive demonstration session, where everyone will be able to view each demonstration and learn from each other.

## Assessment

The grade that a student receives on this assignment will have the following components.

- **GitHub Actions CI Build Status [up to 5%]:**: For lab03 repository associated with this assignment students will receive a checkmark grade if their last before-the-deadline build passes.

- **Mastery of Verbal Explanation during the Demonstration [up to 15%]:**: Since the ability to communicate technical details of a project is crucial to building successful software and hardware applications, a portion of students' lab grade will be determined based on the quality of the project demonstration.

- **Mastery of Technical Writing [up to 25%]:**: Students will also receive a checkmark grade when the responses to the writing prompts presented in the `report.md` reveal a proficiency of both writing skills and technical knowledge. To receive a checkmark grade, the submitted writing should have correct spelling, grammar, and punctuation in addition to following the rules of Markdown and providing complete and conceptually and technically accurate answers.

  - Please note that the "Check Spelling" GitHub Actions check may flag proper nouns or other real words if the dictionary it uses does not contain them. If your "Check Spelling" GitHub Actions check is failing due to a correctly spelled word being incorrectly flagged as "unknown" by CSpell, you will need to add the word to the list of words in `.github/cspell.json`.

- **Mastery of Technical Knowledge and Skills [up to 55%]**: Students will receive a portion of their assignment grade when their project design and implementation reveals that they have mastered all of the technical knowledge and skills developed during the completion of this project. All programs must be inside `src/` directory. As a part of this grade, the instructor will assess aspects of the project including, but not limited to, the correctness of the set up of the robot, the completeness and correctness of the implemented software, the use of effective source code comments and Git commit messages.

All grades for this project will be reported through a student's gradebook GitHub repository.

### GatorGrade

You can check the baseline writing and commit requirements of this project by running department's assignment checking `gatorgrade` tool To use `gatorgrade`, you first need to make sure you have Python installed. If not, please see:

- [Setting Up Python on Windows](https://realpython.com/lessons/python-windows-setup/)
- [Python 3 Installation and Setup Guide](https://realpython.com/installing-python/)
- [How to Install Python 3 and Set Up a Local Programming Environment on Windows 10](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-windows-10)

Then, you need to install `gatorgrade`:

- First, [install `pipx`](https://pypa.github.io/pipx/installation/)
- Then, install `gatorgrade` with `pipx install gatorgrade`

Finally, you can run `gatorgrade`:

`gatorgrade --config config/gatorgrade.yml`

## Assistance

If you are having trouble completing any part of this project, then please talk with the course instructor during the laboratory session. Alternatively, you may ask questions in the Discord channel for this course. Finally, you can schedule a meeting during the course instructor's office hours.
