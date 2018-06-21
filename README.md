# GO-CLI
##### by Bobby Jonathan

Developed as the second stage final assignment of SEA Compfest X

GO-CLI is an transportation application for everyone. GO-CLI conects drivers and users through command-line interface program. For your daily transportation need, GO-CLI make the process of "ride-hailing" for every user easy.  This program also provides user the experience of using GO-CLI command line with intuitive syntaxes.

### Requirements and Installation
GO-CLI.zip and Ruby 2.5.0 are required to run GO-CLI application. The most reccommended operating system for GO-CLI app is Linux and OSX because of the Terminal it has. GO-CLI requires Terminal or Bash Shell because its syntaxes can only be recognized by Terminal.

For Windows, the alternative to Terminal are Linux Bash Shell (Windows 10 and 8) or VirtualBox (Windows 7 and older Windows) with Linux OS installed.

First, download GO-CLI app to start the installation. GO-CLI.zip can be downloaded by clicking the following link (https://github.com/syncopation101/GO-CLI). After that, extract the .zip file somewhere in your PC. Then, install Ruby 2.5.0 if it hasn't been installed by typing Terminal command line written in this link (https://www.ruby-lang.org/id/documentation/installation/).

### Instruction
##### Starting GO-CLI
You can start using GO-CLI by opening GO-CLI folder in the Terminal or Bash. After opening the folder, type this command line to start GO-CLI
```
ruby GO-CLI.rb
```
This command line will start GO-CLI with a 20x20 map with a random user and five random drivers position.

GO-CLI map is designed in nxn square to maximize user's line of sight to all directions.

The other way to use GO-CLI is by determining the n size of the map and x,y position of user with command below
```
ruby GO-CLI.rb n x y
```
where n is the size of map (nxn), x is row position of user, and y is column position of user. x and y is in range of 1 to n to make the usage intuitive for non-programer user. Five drivers will be generated with random position. 

Another yet powerful way to use GO-CLI is by typing the filename in the command line
```
ruby GO-CLI.rb filename.extension
```
GO-CLI is able to open any document file extensions. There is a format that you have to follow so GO-CLi can recognize your input.
```
n user_row user_column m
driver_row_1 driver_column_1
driver_row_2 driver_column_2
.           .
.           .
.           .
driver_row_m driver_column_m
```
n is the size of the map. user_row and user_column denotes user position in column and row. m is the number of drivers available. This first line of input is ended with "Enter" or newline and each input is separated with space. The next m line is drivers' row and column position separated with space. First driver position to m-th driver position is ended with newline.

This way of inputing will make each number distinguishable and make another users, drivers, and developers easy to read your input.

#### GO-CLI interface

