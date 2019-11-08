---
layout: post
title:      "My First Portfolio Project: Friend Generator usig CLI Data gem"
date:       2019-11-04 20:20:33 -0500
permalink:  my_first_portfolio_project_friend_generator_usig_cli_data_gem
---


Hello and welcome to my blog. My name is **OJ** and today I am going to write about how I created my first project(Friend Generator) for my portfolio using a CLI GEM.


**What is a CLI Gem Data ?**

A CLI Gem Data is use to provide data from an external source, whether scraped or via a public API. Data provided must go at least a level deep, generally by showing the user a list of available data and then being able to drill into a specific item.

**Planning my Application. **

Before starting to code this application, my first step was to make a to-do list. This helped me understand the requirements of the app and how I will like to Configure my environment before starting to write code. 

**Generating and setting up a basic gem**

What is a Ruby Gem?

Ruby Gems is a package manager for the Ruby programming language that provides a standard format for distributing Ruby programs and libraries.

Creating a Gem using Bundler

**Step 1** Install your gem in your terminal

bundle gem friend_generator

This gem provides a Command Line Interface(CLI) to data scraped from a public website for user to choose which information they want to get in a list.

**Step 2** Add executable file

let’s call the executable file friend_generator,it must place in a bin directory. This file requires a require_relative *'.lib/friendgenerator'* that allows to load all of the files that are in the lib directory. It must begin to the following line:

*#!/usr/bin/env ruby*

require *`'./lib/friendgenerator'`*

We than create an executable file to load all of the files that are in the lib directory.

FriendGenerator::CLI.new.call

**Step 3**: Get permission

`. ls -lah` #it allows to list all the files in the current directory.
`. chmod +x friend_generator` #Make the file executable

**Step 4**: File requirements

![](https://github.com/ojappah/ojappah.github.io/blob/master/img/1.PNG)


**Step 5**: Explain what it is doing.

I added in the lib/directory two new files: *CLI.rb* and `Friend.rb` file which will also serve as my scraper.

CLI class is a class controller that interacts with the user.  Inside of this controller are:

*#call method*: it is responsible to bundle all methods such as: *#friendoptions*,* #makefriends* and *#exit* methods.

*#friendoptions* and * #makefriends* method allows us to interact with user input.
`#exit` method allows the user to quit the application

The Friend class allows us to grab data from the websites.

[test](http://github.com/ojappah/ojappah.github.io/blob/master/img/image.png)

Output

[test](https://github.com/ojappah/ojappah.github.io/blob/master/img/2.PNG)

[](https://github.com/ojappah/ojappah.github.io/blob/master/img/3.PNG)

My short Video

[My_short_video](http://youtu.be/1eipsbi4lA0)


Thank you for reading. 





