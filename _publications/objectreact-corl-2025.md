---
title: "ObjectReact: Learning Object-Relative Control for Visual Navigation"
collection: publications
category: conferences
permalink: /publication/objectreact-corl-2025
excerpt: 'The paper introduces an object-relative control framework for visual navigation using a relative 3D scene graph, enabling more flexible, embodiment-invariant path planning and control that generalizes better across tasks and real-world environments than traditional image-relative methods.'
date: 2025-09-27
venue: 'Conference on Robot Learning (CoRL)'
paperurl: 'https://arxiv.org/pdf/2509.09594'
# citation: 'Garg, S., Craggs, D., Podgorski, S., Krishna, M., Bhat, V., Dayoub, F., Mares, L., & Reid, I. (2025). "ObjectReact: Learning Object-Relative Control for Visual Navigation." <i>Conference on Robot Learning (CoRL), 2025</i>.'
---

This paper presents **ObjectReact**, a new framework for visual navigation that learns to control a robot relative to *objects* rather than matching camera images. This object-centric approach makes navigation more flexible and robust to changes in the robot's body or sensor setup. Traditional visual navigation methods are often "image-relative," trying to match the current view to a saved subgoal image. This approach is strongly tied to the robot's specific pose and embodiment, making it brittle to changes like variations in sensor height.

ObjectReact overcomes these limitations by using a **relative 3D scene graph** to build a map based on object connectivity. The controller is conditioned on a "WayObject Costmap," which represents the path cost associated with visible objects, completely eliminating the need for a target RGB image. As a result, the system shows high invariance to different robot embodiments and can generalize to challenging new tasks—like navigating a route in reverse or taking shortcuts—that image-relative methods often fail. The policy, trained only in simulation, also generalizes well to real-world indoor environments. 

You can find more details on the [project website](https://object-react.github.io/).