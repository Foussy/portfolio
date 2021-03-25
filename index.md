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

# Project 2 : Finite element analysis viewer
### Python3 | SQL | PyQt5 | pptk | multiprocessing | matplotlib
![pyapod screenshot](images/FEA_viewer.png)

This is a productivity tool I developed working as a Simulation Engineer to dimension aircraft structure. 

At that time, I was doing finite element analysis (FEA) using shell elements (2D element) for carbon composites structures. Doing the post-processing for big model results can be such a time-consuming task in the software I was using at that time (CatiaV5), especially because of poor performances and the lack of options to display results quickly. 

So basically I coded a macro in CatiaV5 that runs the simulation, generates the results and exports all the data in raw text files : x/y/z coordinates for each node, stresses values, composites failure criterion, deformation value, ...

What this software does is to retrieve all the data from the files, sorts & reorganizes them, removes duplicates, etc… And it stores them in a database file. This .db file can then be loaded inside within the program to generate cloud points in a 3D environment using the _pptk_ library.

There are many features to display the different criterions of the simulation, changing the threshold, sorting them in the tables, looking at the different layers of the carbon composites structures, and many others...

This software has been very useful for me as an aircraft engineer.

---

# Project 3 : Snake
### C++ | SFML

![snake screenshot](images/Snake_Game.png)

Well... It's a Snake game.

---

# Project 4 : Game Bot
### Python3 | tkinter | selenium | pytesseract | anticaptcha

![raspberry](images/raspberry.png)

Context : When I was ~13 years old, I started playing an online strategy turn-by-turn game called Lordswm.com. In this game, you can earn virtual money by going into factories and “work” for a certain wage. There is an economic system and since I dug a bit into it, I found a way to entirely automate the process of earning money.

This program was constantly running on my raspberry pi. It is coded in Python3 and uses Selenium library to automate some tasks using a web browser. So basically, every hour, it logs me into the website and performs some specific tasks (finds my location, then available factories sorted by descending wage, downloads a captcha and solves it thanks to an independent OCR service). Using selenium-webscrapping capabilities, It has a virtual market surveillance feature to check if some goods are sold under the general market value. If it is the case, it buys them automatically and put them back in the market instantly for a higher bid.

For further development, I would like to keep track of every catpcha I download and train my own AI to solve them for me. I just started learning about Neuronal Network/Deep Learning and tried to go with Tensor Flow but didn’t have time to pull something out yet.

![captcha](images/captcha.png)

This is not a big OOP project and the GUI is very basic but it is definetely one that I enjoyed a lot because I had very few knowledge of what should be done, and I started sketching from scratch how I should automate stuff, browsing documentations, tinkering a way to get things done. This is why I wanted to add it to the list.

The funny thing is that because I obviously broke some in-game rules, my account has been banned and I am no longer using this script. I guess I deserved it.

---

# Project 5 : Fluid Dynamics
### C++ | Qt | SFML

Work in progress...
