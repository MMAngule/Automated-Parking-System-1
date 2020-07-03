# ***Eklavya 2020 Project Doc***

## **Automated Parking System** --->

This is the project where we use vrep to simulate a parking model and make the car park in different orientations ( namely **Parallel** , **Perpendicular** and **Angled**(usually 45 degrees) )

***
### Table of Contents
***
* [About Project](#About-project)

    * [Aim and Description of Project](#Aim-and-Description-of-Project)
    * [Tech Stack](#Tech-Stack)
    * [File Structure](#File-Structure)
* [Getting Started](#Getting-Started)

    * [Prerequisites](#Prerequisites)
    * [Installation](#Installation)
* [Usage](#Usage)
* [Results and Demo](#Results-and-Demo)
* [Future Work](#Future-Work)
* [Troubleshooting](#Troubleshooting)
* [Contributors](#Contributors)
* [Acknowledgement and Resources](#Acknowledgement-and-Resources)
* [License](#License)
  
***
### About Project
***


#### Aim and Description of Project :
![Parking Model](Parking%20model.png)

We, in this project, have aimed in bringing automation in cars which is already in a developing stage all around the world (Great example is of **Tesla's Self Driving Cars**). Although there are many aspects related to automation but we have focused on achieving a single task (automatic parking) by
integration of sensors and actuators controlled by microcontroller and strategy
planning/coding and for this we have used **Naked Ackermann Model** which is already available in the software

#### Tech Stack :

We have used Coppeliasim Software for our project

* [Coppeliasim]([https://](https://www.coppeliarobotics.com/))

#### File Structure :
    .
    ├── Parallel+Perpendicular(Final Model).ttt                  # Contains the necessary code for parallel and perpendicular parking and their removal
    ├── Images                    # Images
    │   ├── code.png            # Displays Code
    |   ├── Lua.png           # Shows the area where we can see the error or print something from 
    |   ├── parallel_parking.png         # Shows Parallel Parking
    |   ├── parallel_removal.png             # Shows Parallel Removal
    |   ├── parallel_removal2.png           # Leaves the parking space and moves ahead
    |   ├── parallel_turning.png            # Shows the turning of car while parking
    |   ├── Parking model.png           # Shows the Parking Model
    |   ├── perpendicular_parking.png           # Shows the Perpendicular Parking of car
    |   ├── perpendicular_removal.png           # Shows the removal of car by turning
    |   ├── perpendicular_removal2.png          # Leaves the parking slot and moves ahead
    |   ├── perpendicular_turning.png           # Shows turning of car to move inside the parking space
    |   └── script.png          # Shows the name of model with the script icon
    │            
    ├── Project Report.pdf                     # Gives the project report 
    ├── LICENSE
    └── README.md 
    


***
### Getting Started
***

#### Prerequisites :

* [Coppeliasim edu latest version](https://www.coppeliarobotics.com/downloads)
* [Git](https://gitforwindows.org/) 
* [Github for making Repositories](https://github.com/)
  
>How to install these softwares
1. Click on the above "**Coppeliasim edu latest version**" that will redirect you to the downloads section of coppeliasim website and download the edu version of it.
2. Click on the above "**Git**" that will redirect you to the website .
3. Click on the above "**Github for making Repositories**" that will redirect you to the website of github where you to first register yourself and then make repositories

#### Installation :

If you want to take these files from our repository to your system , Clone our Repo by writing this code given below in your git bash

```sh
git clone https://github.com/kart1802/Automated-Parking-System.git 
```

***
### Usage
***

Now in coppeliasim there are main scripts and child scripts, we use child scripts which needs Lua language
You can see after the name there is document type icon which is a script <br>
![Script](script.png)<br>
When you double click and open it you will see the code
![code](code.png)
After running the simulation if you get any error or you want to print something, you will see that in the given box below<br>
![Lua](Lua.png)

***
### Results and Demo
***
The car detects the parking space checks if the condition is satisfied then it
performs the parking function.The car parks itself without colliding with other cars
or the wall with the help of sensors in the front and back as well as the sides

***PERPENDICULAR PARKING*** :<br>
The perpendicular parking takes only one 90° arc

![Perpendicular Turning](perpendicular_turning.png) ![Perpendicular Parking](perpendicular_parking.png)


***PARALLEL PARKING*** : <br>
The parallel parking takes two arcs as explained above for parking

![Parallel Turning](parallel_turning.png) ![Parallel Parking](parallel_parking.png)

***EXIT FROM PARKING LOT*** : <br>

1. **From Parallel** --->

![Parallel Removal 1](parallel_removal.png)
![Parallel Removal 2](parallel_removal2.png)

2. **From Perpendicular** --->
   
![Perpendicular Removal 1](perpendicular_removal.png)
![Perpendicular Removal 2](perpendicular_removal2.png)


Our Video Links -

1. [Parallel Parking and Removal](https://youtu.be/n02HSPTUTH8)
2. [Perpendicular Parking and Removal](https://youtu.be/cG3JKu5vsXQ)


***
### Future Work
***

* [x] Created a desired parking model
* [x] Completed with parallel as well as perpendicular parking
* [x] Completed the removal of a car from parking space as well
* [ ] Need to use obstacle avoidance as well

* [ ] ***Self driving car***<br>
  As we have completed the automated parking sytem of cars , so in future we wish to work on self driving car . We deeply want to study about how cars run on road without any manual input . We are desperate to know , what mechanism goes behind it or how all things works ? It is good thing on which we can make project . By this project we will be unable to know about how self driving cars works . By this project we can understand Tesla cars in detail .
 In this project we can also deeply understand about mechatronics . We also can understand how AI work in self driving cars . By this project we will also understand simulation software deeply .
  We are also curious about knowing how car overcome every barrier on road without any manual input . By this project we would also  learn about mechanics in cars , how engine works . We will also get to know how machine can control speed automatically .
  So in brief , self driving car is really a good project to do as it consists of some wonderful and conceptual things .


***
### Troubleshooting
***
* The removal of car from parallel parking space may turn the car in the direction of parked cars thus raising the chances of a crash to avoid that change value of *dist_rl - dist_fl > 0.55 or 0.575* as for time being we have written the code that works mostly on numbers.
* Also if some sensor has nil value of distance then lua will give an error regarding that , so then added condition like if distance value is not nil something like that and also not use print statements which also give errors

***
### Contributors
***
> Mentors

1. Mr. Manas Thorat :
2. Mr. Saharsh Jain :
3. Mr. Omkar Sargar :
4. Mr. Lukesh :
   
> Members

1. Mr. Karthik Swaminathan : karthikswami.1802@gmail.com
2. Mr. Gaurav Mundada : gauravmundada2001@gmail.com
3. Ms. Mayuri Angule : mayuriangule2727@gmail.com
4. Ms Sanghamitra Ranganathan : ranganathansanghamitra@gmail.com

***
### Acknowledgement and Resources
***

* SRA VJTI Eklavya 2020
* [Vrep Tutorials](https://www.youtube.com/watch?v=PwGY8PxQOXY&list=PLjzuoBhdtaXOoqkJUqhYQletLLnJP8vjZ)

* [CiteSeerX PDF](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.102.1958&rep=rep1&type=pdf)

* [Reseachgate](https://www.researchgate.net/publication/319853826_AUTOMATIC_PARKING_OF_SELF-DRIVING_CAR_BASED_ON_LIDAR14)

***
### License
***