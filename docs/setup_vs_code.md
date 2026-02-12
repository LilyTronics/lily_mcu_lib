# Setup VS code with AVR GCC

This manual describes how to setup VS code with AVR GCC


## Install VS Code

Download and install VS code. Add the following extensions:

* C/C++
* C/C++ Extension pack
* Makefile tools


## Install AVR-GCC

Download the AVR GCC binaries.

https://github.com/ZakKemble/avr-gcc-build

Extract the files in a folder like `C:\avr_tools\avr_gcc`


## Setup the environment

Add the following paths to your environment:

* Add to `Path`: `C:\avr_tools\avr_gcc\bin`
* Create `AVR_GCC_ROOT` : `C:\avr_tools\avr_gcc`

Test the paths. Open a terminal and type the commands:

`avr-gcc --version`
`avrdude --version`


## Create the proper files for VS code

Create a folder called `.vscode`. Copy the following files from this repo:

* `.vscode/c_cpp_properties.json`
* `.vscode/launch.json`
* `.vscode/tasks.json`

Update them to your needs.


## Create a Makefile

Create a makefile for compiling your project.
You can use the make file from this folder as a starting point.

Special attention: Makefile needs tabs for indentation (no spaces)


## Optional tools

Programming GUI for avrdude: https://github.com/ZakKemble/AVRDUDESS
