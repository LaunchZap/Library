Library
=======

a Stylus Mobile-first high-scalable and simple stylesheet for ANY web project.


it requieres:
* Node-js
* Stylus
* nib

If you are not sure you have installed stylus and nib run:

´npm install -g stylus´
´npm install -g nib´

The documentation for Stylus and Nib are in:


http://nibstyl.us/
http://learnboost.github.io/stylus/


Run Stylus specifyng the output folder as:

´cd ~/main/´

´stylus -u nib /source/library.styl --o /css´

You can also use the -w or --watch option to automatically watch your Library files and recompile when any changes are saved.

´stylus -w -u nib /source/library.styl --o /css´
