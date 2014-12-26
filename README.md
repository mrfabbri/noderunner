noderunner
==========

Noderunner is a Node.js app that runs scripts every second, minute, hour or day, each group in its own folder. 

#### How does it work
Copy noderunner.js to a folder with a single sub-folder: scripts. 
In scripts, there are four sub-folders, everySecond, everyMinute, everyHour, overnight and startup. 

Any file with a .js extension in those folders are loaded and run when it's their time. 

All other files are ignored.

The files are not cached, so you can make changes while Noderunner is running.

They share data through a structure called localStorage, which works more or less like localStorage in browsers.
#### Why folders?
I like Dropbox. I've built a few pieces of software over the years based on the idea of storing all the data in folder structures. This means that pieces of the app can easily be distributed among a variety of machines, or easily moved. With folders, I can manage my scripts from any of my Dropbox-capable computers, which includes my desktop, laptop, tablet and smartphone. 
Node.js plus Dropbox-managed folder structures is an incredible combination of technologies in 2015. BTW, when I say Dropbox, I mean all manner of systems that do more or less the same thing, synchronizing folders across devices. 
#### Why did you develop it?
I need it.
#### How do you know it's useful?
This is an adaptation of a couple of core features in Frontier, a scripting and object database environment I led the development of. Now that I'm working primarily in Node, I wanted the same ability to quickly add and edit scripts that are constantly running on net-accessible systems. 


