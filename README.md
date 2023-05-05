# RisikoDL

## The goal is to develop an object detection system for the Risiko! game
(https://en.wikipedia.org/wiki/RisiKo!)

As you may know, in Risiko! game there are two (usually) types of pieces:
tanks and flags.
For this project, you need to design and implement a method for detecting
those two pieces in the YOLO style, i.e., localizing them with a bounding box.
Let’s define with army either a tank or a flag. The problem will consist in the
detection of 12 different classes (6 tanks, 6 flags, each in the different color of
blue, red, yellow, purple, black and green).
Since the collection of a real dataset is prohibitive in terms of time spent in
labelling, you’re given a Jupyter Notebook for producing a synthetic dataset
that will automatically produce and label some data.
By iterating, you can obtain a full synthetic dataset! Then, you just train on it
instead of using big, expensive, real datasets.

So, requirements of this projects are:
1) Produce the synthetic dataset using the Notebook script (if you want, you can modify it!) and split it in Training/Validation/Test
(you’re given also an example of synthetic dataset. Take a look at it, and if you want, integrate it in your synthetic dataset)
2) Split the real images dataset you are provided in Training/Test (70/30 rule)
3) Design a suitable Deep Learning architecture
4) Train the model (first time: only using synthetic training set)
5) Test the model on the test split of the synthetic dataset: report the performance
6) Test the model on the real images that you are provided: report the performance
7) Re-do the steps 4-6 by introducing the real images training set. How does the performance change?
For comparison, you can find a YOLOv7 model (scripts are taken from this repo https://github.com/WongKinYiu/yolov7) trained on this
task. Use the notebook Risiko! Test.ipynb and report the performance of this model on your test set (both synthetic and real) in your project
report.
Try to think how to integrate this system in a fully autonomous player of Risiko! You’ll never lose a match again!
