# Final Project  Deep Learning  CS 7643 - Team Of Mice and Men
Developed and written by: Emilio Moyers, Diana Lomelin, Jonothan Barton, Andres M Menendez.

Full Project is private due to class policy. Please reach out to me for further interest: andmenendez@gmail.com

## Overview
Behavior classifications are difficult and complex problems as the differences between two behaviors can be unnoticeable to even trained scientists. These identifications become particularly difficult when labeling video data as it’s very difficult for a human to determine when one behavior begins and ends on a frame-by-frame basis. Deep neural networks can solve this classification issue as they are more consistent and are unequivocally faster than any human. With a plethora of different available modules and tools, it can be difficult to design and train the right architecture for the right model. These networks will have to take into account the temporal nature of this behavior classification as a single behavior can best be identified through its context and not solely concerning a single frame. 

For more information about the implementation, please refer to the [paper](https://github.com/andmenendez/Final-Project-Deep-Learning-CS-7643---Team-Of-Mice-and-Men/blob/main/Final_Project_CS_7643.pdf).

## Original Test and Training sets

The original train and test set for Task1 and Task3 can be accessed in the following links: [Task1](https://www.aicrowd.com/challenges/multi-agent-behavior-representation-modeling-measurement-and-applications/problems/mabe-task-1-classical-classification/dataset_files), [Task 3](https://www.aicrowd.com/challenges/multi-agent-behavior-representation-modeling-measurement-and-applications/problems/mabe-task-3-learning-new-behavior/dataset_files).

## Folder and Important Files Description

In the next sections, you can find a brief description of the folder and important files.

### Folder

* Documents: contains the final paper for the project.
* Diagrams: contains diagrams of the pipelines used in the project, used when writing the paper.
* Models: contains the implementation of the Neural Network models we tried, during the development and experimentation phase of the project.
* Modules: contains losses and schedulers implementations.
* Scripts: contains scripts used to download the datasets from AIcrowd platform.

### Important Files

* data.py : file that contains the code for the data generator used by the data loaders (task 1 and task 3).
* main_ensemble_task1.py : main file that contains the code for the ensemble using best Transformer and best CNN model (task 1).
* main_noisy_student.py : main file that contains the code for the generation of pseudo labels using an unlabeled data set, and the training loop using the original training set and new pseudo labels set (task 1).
* main_task_unsup.py: main file that contains the code for the unsupervised training using the training set and test set as unlabeled sets, and contrastive loss as the loss function (task 1).
* main_task3.py: main file that contains the code for the unsupervised training using the training set and test set as unlabeled sets, and contrastive loss as the loss function (task 3).
* main_teacher_student.py: main file that contains the code of the teacher-student knowledge distillation training (task1).
* main.py: main file that contains the code for the normal supervised training (task 1).
* train.py file contains the code for the training loop and a little more (task 1 and task 3).

## Other important links 

* [Link](https://drive.google.com/drive/folders/1PUbMx9r1lN5rm3WlzD6nSW5IQnziznQa?usp=sharing) to some of our trained models. You can download them from the link provided if you want to verify or play with our experiments.
* Links to AIcrowd submission board, in case you want to verify the result we repot on the paper: [Task 1](https://www.aicrowd.com/challenges/multi-agent-behavior-representation-modeling-measurement-and-applications/problems/mabe-task-1-classical-classification/submissions) and [Task 3](https://www.aicrowd.com/challenges/multi-agent-behavior-representation-modeling-measurement-and-applications/problems/mabe-task-3-learning-new-behavior/submissions). The submissions for out team can be under the names: **andres_menendez**, **dianalomelin**, **emilio_moyers** or **gnodabb**.

