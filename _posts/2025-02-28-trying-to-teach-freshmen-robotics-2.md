---
layout: post
title: Trying to Teach Freshmen Robotics 2
date: 2025-02-28 16:00:00
description: My introduction to robotics for a few undergrad freshmen
tags: IIIT robotics
categories: robotics
---

## Weeks 5 to 8

### Stuff that I sent over

1. PyTorch  
2. Robotic Vision (with OpenCV)

Evidently, progress in the stuff I could teach was slow owing to academics (ironic, isn't it?). Regardless, they are still interested in RRC and a couple of them got part-time internships in a robotics startup (Yay!).

### PyTorch

Not just the basics but also dive into critical aspects that will be essential for applying neural networks to robotics problems.

1. **Getting Started with PyTorch:**  
   - **Resource:** [Deep Learning with PyTorch: A 60 Minute Blitz](https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html)  
     Familiarize yourself with the core components of PyTorch.

2. **Data Loaders and Datasets:**  
   - PyTorch’s `torch.utils.data.Dataset` and `DataLoader` classes are designed to simplify data handling.  
   - **Key Aspects:**  
     - **Custom Datasets:** How to structure and preprocess your robotics data for training.  
     - **Batching & Shuffling:** Efficiently loading data during training to improve performance.  
     - **Parallel Data Loading:** Leveraging multi-threading to accelerate your training pipeline.  
   - **Resource:** The [Data Loading Tutorial](https://pytorch.org/tutorials/beginner/data_loading_tutorial.html)

3. **Optimization Theory:**  
   - Understanding the mathematics and intuition behind optimization is crucial.  
   - **Focus Areas:**  
     - **Gradient Descent and Variants:** Learn why and how different optimizers work (SGD, Adam, etc.).  
     - **Tuning Hyperparameters:** Experiment with learning rates, momentum, and other parameters through `torch.optim`.  
   - **Resource:** The [PyTorch Optimizers Documentation](https://pytorch.org/docs/stable/optim.html) is a solid starting point.
   - **Other stuff:**
     - You have done quite a bit of this in the mathy bits earlier and will redo it in the mobile robotics course. Take a look again at this in for the time being: [Intro to Optimization](https://web.stanford.edu/group/sisl/k12/optimization/MO-unit1-pdfs/1.1optimization.pdf)

### Robotic Vision with OpenCV

1. **Introduction to OpenCV:**  
   - **Resource:** The [OpenCV-Python Tutorials](https://docs.opencv.org/master/d6/d00/tutorial_py_root.html) for an overview.

2. **Multi-view Geometry:**  
   - A super important thing in robotic vision is the ability to perceive depth and spatial relationships using multiple images.  
   - **Focus Areas:**  
     - **Camera Calibration:** Learn to determine intrinsic and extrinsic camera parameters to correct lens distortions.  
       - **Resource:** The [Camera Calibration Tutorial](https://docs.opencv.org/3.4/dc/dbb/tutorial_py_calibration.html) guides you through this process.  
     - **Epipolar Geometry & Stereo Vision:** Understand how to estimate depth and recover 3D information from two or more camera views.  
       - **Resource:** [Multi-view Geometry](https://www.robots.ox.ac.uk/~vgg/hzbook/) is perhaps the best book available. There are a few copies in the library as well.

3. **Robust Vision Pipelines:**  
   - **Key Concepts:**  
     - **Feature Detection:** Experiment with detectors such as SIFT, SURF, or ORB to recognize and match key points in images.  
     - **Real-time Processing:** Build pipelines that can handle continuous video streams and process images on the fly.

#### Final Things

Once you're done. Start with reading about SLAM pipelines.
