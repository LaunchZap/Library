Library
=======

a Stylus Mobile-first high-scalable and simple stylesheet for ANY web project.


it requieres:
* Node-js
* Stylus
* nib

If you are not sure you have installed stylus and nib run:

	npm install -g stylus
	npm install -g nib

The documentation for Stylus and Nib are in:


http://nibstyl.us/
http://learnboost.github.io/stylus/


to install Library in your project, you can download it or clone the repository as a submodule in your project.
If you install it as a submodule, you will have EVER the latest version

Note: the [main]$ bits on each line represents your bash prompt. You should only type the stuff after the $.


Set up the submodule for the first time:

	[~]$  cd ~/main/
	[main]$  git submodule add git://github.com/launchzap/library.git ./library
	[main]$  git submodule update --init
	[main]$  git commit ./library -m "Added submodule as ./css"


If you want to actualize the submodule
	git submodule foreach git pull


Run Stylus specifyng the output folder as:


[~]$cd ~/library/
[main]$ stylus -u nib /source/library.styl --o /css


You can also use the -w or --watch option to automatically watch your Library files and recompile when any changes are saved.


[main]$ stylus -w -u nib /source/library.styl --o /css


