# Assignment-2

CS361: Assignment 2: Microservices Warm-Up

Overview
To demonstrate you can implement the microservices architecture, write software comprised of three separate programs:
A program that generates pseudo-random numbers (PRNG Service)
A program that, given a non-negative integer i, returns the ith image in a set (order doesn’t matter) (Image Service)
If i is >= the number of images, modulo i by the size of the image set
A user interface (UI) that either has a button or can receive a user command. When the button is pushed or the command is entered...
UI calls the PRNG Service
UI calls the Image Service using the pseudo-random number from the PRNG Service
UI displays the image (or a path to it) 

Programs can be written in any language(s).

Use any set of images (e.g., downloaded from https://www.kaggle.com/). Store images locally in a folder; no API calls needed. No DB needed.

Requirements
UI must either have a button (if UI is graphical) or be able to receive a user command (if UI is text-based)
Each of the three programs must run in a different process
Programs must NOT call each other directly (e.g., do not import one program into another)
As the communication pipe, use text files as follows:
UI calls PRNG Service by writing the word "run" to prng-service.txt
PRNG Service reads prng-service.txt, erases it, and writes a pseudo-random number to it
UI reads prng-service.txt to get the pseudo-random number


UI writes the pseudo-random number to image-service.txt
Image Service reads image-service.txt, erases it, and writes an image path to it
UI reads image-service.txt then displays the image (or path) to the user
Create a short video (5 minutes or less) demonstrating you have satisfied the require- ments.

Submission
Embed or link to video.
For video, you must follow instructions at Modules > “HOW TO: Create and Upload a Video”.

Grading
You are responsible for satisfying all criteria listed in the Canvas rubric for this assignment. You will be able to revise this assignment if you miss points.

Questions?
Please ask via Ed so that others can benefit from the answers.
