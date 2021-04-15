# project 1 : [pyapod](https://github.com/Foussy/pyapod)
## Python3 | PyQt5

![pyapod screenshot](images/pyapod.png)

This software is a cross platform front-end of the [Astronomy Picture Of the Day website](https://apod.nasa.gov/apod/astropix.html) posting Space related photos & videos everyday since June 1995. It is designed with python3 and PyQt5 and it uses the API developped by NASA.

Main features :
* Loading and rezising dynamically the images from the API. 
* Opens up today’s picture
* Possibility to change the date backward/forward, select a specific or a random one.
* Title, date, description and copyrights displayed of the bottom textbox.
* Dark theme for better aesthetic and consistency with Space.

Features in developement :
* Favorites menu
* Cache manager to enhance performance when loading and resizing images

I developed this project mainly because I like apod a lot and I regularly kill some time browsing pictures and reading about Space on it. It was a good introduction to start learning about APIs.

---

# project 2 : [Finite element analysis viewer](https://github.com/Foussy/DTC_Workflow_Calcul_Avion)
## Python3 | SQL | PyQt5 | pptk | multiprocessing | matplotlib
![pyapod screenshot](images/FEA_viewer.png)

This is a productivity tool I developed working as a simulation engineer. In simple words, its purpose is to recover data extracted from CATIA V5's calculations, and display them in the most efficient and practical way for an engineer to analyze the results and utilize it as a decision maker.

At that time, I was doing finite element analysis (FEA) using shell elements (2D element) for carbon composites structures. This type of structures can be described as a multi-layered oriented stacks of carbon fibers. Doing the post-processing for big model results can be such a time-consuming task in CATIA V5, because some structures I was designing could contain many layers (up to 50) and I had to look in each one of them for the critical nodes (my biggest model contained 1 million nodes). Moreover, the software offered poor performances for this specific task.

Eventually, I came up with this workflow :
* After I was satisfied with a design, I was running a python script to manage the inputs of my model (.xml) and give it to CATIA
* I would then launch a macro in CATIA that launches the computation, generates the results and exports all of it in raw text files
* From this text files, I would use the software to recover x/y/z coord for each node of the mesh, the stress tensor, deformations, specific composites failure criterion (Hashin, Tsai-Wu, Puck...)
* The software then sorts & reorganizes the results, removes the duplicates and the unwanted nodes. 
* It stores them in a .db file which can then be loaded within the program to generate colorized cloud points in a 3D embedded window (_pptk_).

There are many features to this program, like the possibility to change the color threshold, to sort the point in tables which directly interact with the 3D window, to quickly and smoothly switch from one carbon layer to the other, and many others...

This software has been very useful for me and my team. 

---

# project 3 : [Game bot](https://github.com/Foussy/Lords_labour)
## Python3 | tkinter | selenium | pytesseract | anticaptcha

![raspberry](images/raspberry.png)

Context : When I was ~13 years old, I started playing an online strategy turn-by-turn game called Lordswm.com. In this game, you can earn virtual money by going into factories and “work” for a certain wage. There is an economic system within the game and since I dug a bit into it, I found a way to entirely automate the process of earning money.

I was running this programm on my raspberry pi. What it does is :
* Every hour, it opens up a web browser using Selenium and logs me into the website.
* Then it performs some specific game tasks : find the location of my character, find factories with free slots sorted by descending wage, download a captcha and solve it (using OCR service). 

I also added several improvements like a market surveillance feature to check if some goods were sold under a threshold value I would fix. It would buy them and automatically put them back in the market for a higher bid.

For further development, I was keeping track of every captcha I was downloading to train my own AI. I started learning about neuronal network and went with tensor flow but I eventually got my account closed for exploiting the game. Anyhow I had a lot of fun doing this project, because I had so few knowledge of everything. I spent a lot of time searching for documentations, browsing and tinkering a way to get things done. This is definetely not a big OOP project and the GUI is ugly, but this project is among my first ones and I liked every bit of it. This is why it is in the list.

![captcha](images/captcha.png)

---

# project 4 : [py-schach](https://github.com/Foussy/py-schach) (chess game)
## Python | pygame

![pyschach](images/pyschach.png)

Still in development, the game mechanics are not fully implemented.

---

# project 5 : Fluid dynamics
## C++ | Qt | SFML

This is my first big project in C++. This project is currently in progress. Its goal is to display 2D fluid fluently, to be able to play with it with inputs like mouse motion, add dye inside it to see the various effect of the Navier-Stokes equations, display the velocity field, etc... This project has been inspired by [this website](https://paveldogreat.github.io/WebGL-Fluid-Simulation/). I am really impressed about how fast the animation is while I know doing CFD with FEA softwares can quickly take huge amount of ressources and time to compute. After doing some researches, it is because this kind of programs tend to approximate solutions for Navier-Stokes. Its purpose is not to be accrurate scientificaly speaking, but instead it is just to look good and uses few resources. This is what developers use for rendering fluids in games or animation movies. If you want to know more about it, check out this paper written by Jos Stam : [Real-Time Fluid Dynamics for Games](https://www.dgp.toronto.edu/public_user/stam/reality/Research/pdf/GDC03.pdf).


I already coded the program in python, but it is slow and kind of bugy with pygame. Feel free to look at the [my github repo](https://github.com/Foussy/Fluid_Dynamics/blob/master/Field.py). I am currently refactoring the code for C++.

---

# project 6 : [Snake](https://github.com/Foussy/Snake)
## C++ | SFML

![Snake](images/Snake_Game.png)

Apart me going through Project Euler problems with C++, this is my first program in C++. Well, it's just a Snake Game, but it is functional !

---

# project 6 : Harmonic Movements
##  Python | tkinter

![Harmonic](images/Harmonic_movements.png)

My first project as I was learning OOP.
