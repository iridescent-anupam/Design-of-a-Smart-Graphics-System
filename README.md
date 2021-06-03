# Design-of-a-Smart-Graphics-System

The modern graphics systems are heavily dependent on a centralized processing unit (GPU) which takes a considerable toll on the performance and provides no intelligent way to draw required images.

In this project we aim to resolve this issue by making our graphics system divide its entire task of processing into several connected processing units each taking up the place of a pixel. Thus every pixel serves to be its own unit that feeds data to the next pixel as required, making it intelligent.

![image](https://user-images.githubusercontent.com/47811736/120631333-63dc2b80-c485-11eb-8391-31f226fbda85.png) (Overview of the Graphics System) 

Instead of depending on one or more centralized processing units, the pixels decide to which neighbouring pixel the control should be transferred to.
The input provided is used to calculate some pre-computed data, to be done by the CPU and then use them as heuristic.
This puts significantly lower strain on the CPU and makes the process faster as it is implemented on a hardware level.

![image](https://user-images.githubusercontent.com/47811736/120631432-8110fa00-c485-11eb-8346-ad9ac1731b86.png) (Structure of a Pixel)
