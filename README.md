Library
=======

a Stylus Mobile-first high-scalable completely customizable and simple stylesheet for ANY web project.

it requieres:
* Node-js
* Stylus
* nib

## Requs install

If you are not sure you have installed stylus and nib run:

	npm install -g stylus
	npm install -g nib

The documentation for Stylus and Nib are in:

http://nibstyl.us/

and

http://learnboost.github.io/stylus/

## Library Install

to install Library in your project, you can download it or clone the repository as a submodule in your project.
If you install it as a submodule, you will have EVER the latest version as long as you made a foreach pull

Note: the [launchzap]$ bits on each line represents your bash prompt. You should only type the stuff after the $.


Set up the submodule for the first time:
	
	[yourprojectpath]$  cd ~/launchzap/
	[launchzap]$  git submodule add git://github.com/launchzap/library.git ./library
	[launchzap]$  git submodule update --init
	[launchzap]$  git commit ./library -m "Added submodule as ./css"


If you want to actualize the submodule

	git submodule foreach git pull

Run Stylus specifyng the output folder as:


	[~]$cd ~/library/
	[launchzap]$ stylus -u nib ./source/library.styl --o ./css


You can also use the -w or --watch option to automatically watch your Library files and recompile when any changes are saved.


	[launchzap]$ stylus -w -u nib ./source/library.styl --o ./css


##UNITS

Some of the most important changues in the CSS can be performed in ~/library/sources/units.styl



##GRID

Library have a a fully customiz­able grid with a zero amount of code for you.
This grid system is loosely based off of the Foundation Twelve Column Grid, with a few important differences:

The absence of grid rows. While they can provide more layout options, grid rows are often times difficult to implement in a dynamic system, where the grid elements are constantly changing.
Simplification. This grid provides a simple, "n" column structure that can be quickly implemented and modified. Let’s keep things light weight!

	<div class="l_grid">
	  <div class="small_6 med_4 large_3 l_column">...</div>
	  <div class="small_6 med_4 large_3 l_column">...</div>
	  <div class="small_6 med_4 large_3 l_column">...</div>
	  <div class="small_6 med_4 large_3 l_column">...</div>
	</div>