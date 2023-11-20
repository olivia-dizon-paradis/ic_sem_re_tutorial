# IC SEM RE Tutorial using AI
In this tutorial, we will be using artificial intelligence (AI) to help reverse-engineer (RE) an integrated circuit (IC) from a scanning electron microscope (SEM) image for hardware assurance. We invite you to follow along with this tutorial and build your own project. We hope this project will serve you well as a resume-booster when applying for a job or further education, or professional development to support your existing position. This module will cover python as a programming language for AI, image processing and computer vision, and machine learning.

## Description
The main goal of this project is to automatically segment the foreground structures of the IC (i.e. the regions of interest) from the background. To accomplish this, we need to take in a grayscale image of an IC and then generate a binary image where the forground pixels are distinctly marked from the background pixels (as shown below). This information can be used to help reverse-engineer the IC.   

![image](./readme_images/goal.png)

This tutorial is divided into four parts:
1. Part 1 sets up our code pipeline for the project
    - Reading and showing images
    - Applying simple thresholding as a naiive segmentation technique
    - Evaluating segmentation results using intersection-over-union (IoU) score
3. Part 2 introduces some topics in Image Processing and Computer Vision
    - Preprocessing using mean filtering 
    - Improving upon simple thresholding using Otsu's method
    - Postprocessing segmentation results using binary opening and closing 
4. Part 3 introduces some topics in Unsupervised Machine Learning
    - Extracting features using blurring, edge detection, and corner detection techniques
    - Segmentation using unsupervised K-means clustering
    - Using cluster centers to understand the k-means clustering algorithm 
6. Part 4 introduces some topics in Supervised Machine Learning
    - Understandin the importance of model generalization incorporating a train/test split 
    - Segmentation using supervised decision tree classification 
    - Segmentation using supervised random forest algorithm to try to achieve better generalization than just one decision tree 

## Installation
Code was tested on Python 3.10.13. To install dependencies, please run

  > pip install -r requirements-3.10.13.txt

on a virtual environment.

## Authors and acknowledgments
- Olivia P. Dizon-Paradis
- David S. Koblah
- Ronald Wilson
- Domenic Forte
- Damon L. Woodard

## Project status 
Completed, pending release
