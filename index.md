# Project 1 : pyapod
### Python3 | PyQt5
![pyapod screenshot](images/pyapod.png)
This little software is a cross platform front-end of the [Astronomy Picture Of the Day website](https://apod.nasa.gov/apod/astropix.html). Posting Space related photos & videos everyday since June 1995. It is designed with python3 and PyQt5 library and it uses the API developped by NASA.


Main features :
* Loading and rezising dynamically the images from the API. 
* Opens up today’s picture
* Possibility to change the date backward/forward, select a specific or a random one.
* Title, date, description and copyrights displayed of the bottom textbox.
* Dark theme for better aesthetic and consistency with Space.

Features in developement :
* Favorites menu
* cache manager to enhance performance when loading and resizing images

I developed this app mainly because I like APOD a lot and I regularly spend some time browsing
cool pictures and reading stuff about Space. It was a good introduction to APIs, how they work, etc...

---

# Project 2 : Fluid Dynamics
### C++ | Qt | SFML
Work in progress...

---


# Project 3 : Finite element analysis viewer
### Python3 | SQL | PyQt5 | pptk | multiprocessing | matplotlib
![pyapod screenshot](images/FEA_viewer.png)

This is a productivity tool I developed working as a Simulation Engineer to dimension aircraft structure. 

At that time, I was doing finite element analysis (FEA) using shell elements (2D element) for carbon composites structures. Doing the post-processing for big model results can be such a time-consuming task in the software I was using at that time (CatiaV5), especially because of poor performances and the lack of options to display results quickly. 

So basicaly I coded a macro in CatiaV5 that runs the simulation, generates the results and exports all the data in raw text files : x/y/z coordinates for each node, stresses values, composites failure criterion, deformation value, ...

What this software does is to retrieve all the data from the files, sorts & reorganizes them, removes duplicates, etc… And it stores them in a database file. This .db file can then be loaded inside within the program to generate cloud points in a 3D environment using the _pptk_ library.

There are many features to display the different criterions of the simulation, changing the threshold, sorting them in the tables, looking at the different layers of the carbon composites structures, and many others...

This software has been very useful for me as an aircraft engineer.

---

# Project 4 : Snake
### C++ | SFML
![snake screenshot](images/Snake_Game.png)
