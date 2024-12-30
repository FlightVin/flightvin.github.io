---
layout: post
title: Trying to Teach Freshmen Robotics
date: 2024-12-25 16:40:16
description: My introduction to robotics for a few undergrad freshmen
tags: IIIT robotics
categories: robotics
---

# Introduction

I recently undertook the task of introducing a bunch of freshmen to robotics. I'll keep updating this as they progress.

The following is a summary of my conversations via text using an LLM.

## Phase 1: Getting Started

### Introductory Topics:

1. **An Introduction to Abstraction** ([Link](https://www.lesswrong.com/posts/CHSBRLWY5bzZdchFF/a-thorough-introduction-to-abstraction))
2. **Writing Modular Code** ([Link](https://best-practice-and-impact.github.io/qa-of-code-guidance/modular_code.html))
3. **Python for Research** ([Link](https://rits.github-pages.ucl.ac.uk/doctoral-programming-intro/)) - Skim the headings to ensure you know the general concepts.

### Dual Boot and ROS Installation:

1. Set up dual boot with **Ubuntu 20.04** (make sure the version matches).
2. Install ROS following the instructions for [**Noetic**](https://wiki.ros.org/noetic/Installation/Ubuntu).
   - If you're adventurous, try Zorin OS. Its installation is similar to Ubuntu.
3. For a modern approach, consider **Docker**. While dual booting is recommended for ROS, Docker is a valuable and intriguing tool worth exploring.
   - Helpful Resources:
     - [Link 1](https://roboticseabass.com/2021/04/21/docker-and-ros/)
     - [Link 2](https://www.reddit.com/r/ROS/comments/19d3fgk/running_ros_in_docker_pros_and_cons/)

**Estimated Time:** 1 day

#### Alternatives to Dual Boot:

- Use a Virtual Machine (VM) as per [this discussion](https://answers.ros.org/question/355252/can-ros-run-smoothly-on-vm/).
- Avoid WSL as it may not fully support ROS.

## Phase 2: Starting Off with ROS

### Fundamental Introduction:

1. Navigate to [The Construct](https://app.theconstruct.ai/courses/) and find the "**ROS Basics in 5 Days**" course (choose either C++ or Python).
   - Note: This course isn't entirely free, but you can access some content for free. It should take about 2 hours.

### Exploring the Documentation:

1. Familiarize yourself with the official [ROS Noetic documentation](https://wiki.ros.org/noetic).
2. Read:
   - [Introduction to ROS](https://wiki.ros.org/ROS/Introduction)
   - [Beginner Tutorials](https://wiki.ros.org/ROS/Tutorials): Complete "**1.1 Beginner Level**" and up to "**5 Defining Custom Messages**" in the "1.2 Intermediate Level" section.

### Key Focus Areas:

- Topics
- Services
- Visualization tools (e.g., RViz)

## Phase 3: Exploring Gazebo

1. Install and read about Gazebo from the [Guided B Tutorials](https://classic.gazebosim.org/tutorials?cat=guided_b&tut=guided_b1).
2. From the [Getting Started page](https://classic.gazebosim.org/tutorials?cat=get_started), explore:
   - Quick Start
   - Gazebo Components
   - Gazebo Architecture
3. Build a robot model ([Tutorial](https://classic.gazebosim.org/tutorials?tut=build_robot&cat=build_robot))
4. Add a sensor to the robot ([Tutorial](https://classic.gazebosim.org/tutorials?tut=add_laser&cat=build_robot))
5. Attempt this project: [YouTube Tutorial](https://www.youtube.com/watch?v=594Gmkdo-_s)
   - Use LLMs (e.g., Perplexity) to convert ROS2 commands to ROS-compatible ones.
   - Download project files from the video description.

## Phase 4: Introducing Machine Learning

### Essential Reading:

1. [A Short Introduction to Machine Learning](https://www.lesswrong.com/posts/qE73pqxAZmeACsAdF/a-short-introduction-to-machine-learning)
   - I highly recommend this, given my affinity for LessWrong's content.
2. [Mathematics for Machine Learning](https://mml-book.github.io/)
   - Quickly review the linear algebra sections before diving into the rest of the book.

**Estimated Time:**
- Brief review: 2-3 days
- In-depth study: 2 weeks (2 hours daily)

### Next Steps:

Once you've completed this, reach out to begin with PyTorch. This book forms the foundation for understanding ML, so take it seriously.

And then, I'll get them started off on computer vision and mobile robotics.
