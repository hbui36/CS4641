## Project Proposal

### Introduction

Many communites in Africa are regularly impacted by movements of certain wildlife populations. We propose that a machine learning model could be used in coordination with motion-activated camera traps to identify movements of certain wildlife populations and understand when these populations might pose a risk to these communities.

### Problem Definition

1. Facilitate foreign conservation groups identifying animals.

2. Problems with animal conservation:
   - Human disturbance on habitat and environment
   - Conflict with community and wildlife:
     - Elephants interfere with crops, community harms elephants
     - Lions getting close to communities
   - Large areas that require a lot of manpower to keep track of
   - **When** and **Where** are the wildlife population?
   - Focusing on African Wildlife. Can be apply to any wildlife in any habitat with training?
   - Help with identification/tracking of animals in an area, estimation of population. Automize of data analytics to feed into other programs.
   - Create a network of cameras that can be maintained by the community. Whenever the camera is triggered by motion, an image is taken

### Methods

- Use of African wildlife data set
- Unsupervised learning - given an unkown object (no label)
  - Object detection
  - Object segmentation
  - Clustering similar images together
  - Distance Estimation
- Supervised learning - identify what type of animal is in the image
  - Neural network - VGG(neural network framework), darknet YOLO v4 - Feed image in, convert image to matrix and try to find patterns, output animal classification
- Probably start with just classification, and then consider moving forward

### Potential Results

We expect our potential results to be accurate categorization of animals detected in the camera as well as an expected distance between the animal and the camera.

Our algorithm will firest detect movement of objects and classify animal movement from non-animal movement. If an animal is detected, the algorithm will accurately provide the animal species. Our results will focus on the 4 animals including: elephant, buffalo, rhino, and zebra. We will enlarge our results to include more wildlife animals if we have time. Concurrently, the algorithm will also provide an approximation of how far the animal is to the camera.

### Discussion

Our program will detect the animal in the image and catalogue it. This data will be used for the position of the animal to inform the community if any actions needs to be taken. For example, if an elephant is detected near a crop field, inform the community to re-enforce the walls around the field. If a lion is detected near a settlement, inform the community to increase the guard shifts.

This data will also allow conservation groups to keep track of animal population in an area without constantly disturbing the environment.

The trained ML model will be evaluated for its accuracy and we aim to achieve at least 95% accuracy. The erros will be looked at and evaluated as why it might be the cause, for example, due to colour or shape similarity.

### References
