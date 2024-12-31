---
layout: post
title: Trying to Teach Freshmen Robotics 1
date: 2024-12-25 16:40:16
description: My introduction to robotics for a few undergrad freshmen
tags: IIIT robotics
categories: robotics
---

_Edit_: Rephrasing

## Week 1: introduction and getting your hands dirty on software

I recently undertook the task of introducing a bunch of freshmen to robotics. I'll keep updating this as they progress.

Here's the first email that I had sent to a mentee (with some bits removed).

---

A short introduction - I'm Vineeth, a UG4 CSE Honours student under Prof. Madhava Krishna. I've worked on Visual Place Recognition, Video Object Detection, Object Identification and Localization, and am currently focused on building a navigation stack (lots of robotics terms - you'll learn them as you go).

Considering that you probably won't be doing courses such as DASS and ISS (_some introductory courses for CS majors at IIIT on software_) that give you a glance into Software Engineering, and since it is vital part of running any experiment successfully, I would like to get you started off with reading the following (skim, don't go much in-depth):

1. An Introduction to Abstraction ([link](https://www.lesswrong.com/posts/CHSBRLWY5bzZdchFF/a-thorough-introduction-to-abstraction))
2. Writing Modular Code ([link](https://best-practice-and-impact.github.io/qa-of-code-guidance/modular_code.html))
3. Python for Research ([link](https://rits.github-pages.ucl.ac.uk/doctoral-programming-intro/), please skim this - see the headings and figure out whether you know the general information in it)

I expect this to take 2-3 days at most, and will then give you resources for:

1. ROS (Please dual boot with Ubuntu 20 for this; If you use some other Linux Distro, check compatibility)
2. Basic Optimization Theory (Brush up on your linear algebra for this)
3. Neural Networks and DL (Basics of ML)
4. Post this, I would like to introduce you to some concepts in computer vision (such as camera matrices, key-point descriptors, multi-view geometry, etc.), take you into larger networks such as CNNs & Transformers, and SLAM.

---

### Installing ROS

1. Set up dual boot with Ubuntu 20.04 (make sure the version matches).
2. Install ROS following the instructions for [Noetic](https://wiki.ros.org/noetic/Installation/Ubuntu).
   - If you’re adventurous, try Zorin OS. Its installation is similar to Ubuntu.
3. For a modern approach, consider Docker. While dual booting is recommended for ROS, Docker is a valuable and intriguing tool worth exploring.
   - [Resource 1](https://roboticseabass.com/2021/04/21/docker-and-ros/)
   - [Resource 2](https://www.reddit.com/r/ROS/comments/19d3fgk/running_ros_in_docker_pros_and_cons/)

## Week 2: getting started with ROS

### A very, very gentle introduction

Check [this](https://app.theconstruct.ai/courses/) out. Find the “ROS Basics in 5 Days” course (choose either C++ or Python) - this course isn’t entirely free, but the parts that are very nicely explain the fundamental uses (and quirks) of ROS.

### Reading the docs

Familiarize yourself with the official [ROS Noetic documentation](https://wiki.ros.org/noetic). Read

- [The introduction](https://wiki.ros.org/ROS/Introduction), and,
- [The Beginner Tutorials](https://wiki.ros.org/ROS/Tutorials): Complete “1.1 Beginner Level” and up to “5 Defining Custom Messages” in the “1.2 Intermediate Level” section.

While doing this, you should be putting a particular emphasis on _topics_, _services_ and _visualization tools_.

## Week 2: The next bits - Gazebo

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

## Weeks 3 and 4: MLLLLL

### Essential Reading

1. [A Short Introduction to Machine Learning](https://www.lesswrong.com/posts/qE73pqxAZmeACsAdF/a-short-introduction-to-machine-learning)  
   - I highly recommend this, given my affinity for LessWrong's content.

2. [Mathematics for Machine Learning](https://mml-book.github.io/)  
   - Quickly review the linear algebra sections before diving into the rest of the book.  
   - Linear algebra is incredibly cool—not just for ML, but also for robotics! Concepts like transformations, projections, and matrix factorizations are the backbone of everything from optimizing neural networks to understanding camera geometry in robotics. A strong foundation in linear algebra, optimization, and related math ensures you're well-equipped to tackle complex problems in both fields.

How much time should it take you?

- Brief review: 2-3 days
- In-depth study: 2 weeks (2 hours daily)

#### Next Steps

Once you've completed this, reach out to begin with PyTorch. This book forms the foundation for understanding ML, so take it seriously.
