# EvolutionSimulator
Simple evolution simulator in C# with Unity

This project was my A.P. Computer Science Priniciples project (I got a 4, I think it was the multiple choice part that got me). I made this in Unity after learning about the method of learning for neural networks called a genetic algorithm. 

Even though the graphics are not the best, and the physics could use some work, it achieves what it is supposed to for the most part.

How the program works is as follows: 
There are 1,000 creatures in each generation. Each creature is made of muscles (gray rectangles) and neurons (white circles). The placement of neurons is random as well as the amount of neurons. Each neuron then randomly connects to other neurons via muscles. Every single neuron has a neural network that controls it, with a bunch of different inputs about its locataion, speed, and other factors going into it. The ouptut is the extension of a given muscle. Since each muscle has two neurons attached to it, the extension amount is averaged between the two controlling neurons. 
The goal of every creature is to move the furthest it can to the right (based on the average position of every neuron) in 15 seconds. A generation then will sort itself by the most fit creatures (top 500 that moved the furthest to the right) and will 'kill' off the lowest 500. From the top 500, random mutations such as removing or adding a neuron will occur, as well as chaning numbers in neurons neural networks occur. 
Clicking on the most fit, median fit, and least fit of a generation will display that creatures run as well as past the 15 seconds it was scored on.

A tendency of this program is that beginning creatures who score high usually do because they flop to the right, causing the average to shift to the right which is technically the goal. Over a few generations these get removed in favor of creatures actually moving. Sometimes sadly creatures abusing the fact that extremely small movements can move them when realistically they would not move come about and take over generations. Other times though, you really can see creatures walking.
