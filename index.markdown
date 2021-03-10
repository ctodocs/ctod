---
title: Welcome & Setup
layout: default
nav_order: 1
---
<<<<<<< HEAD
# Welcome to Committing to Documentation!
Follow the instructions and review the schedule below in advance of the workshop to ensure your system is all set.

# Setup instructions
Follow the below instructions prior to the workshop to ensure that your system is ready for the activities.

* Install [Visual Studio Code](https://code.visualstudio.com/) 
* Create a [GitHub](http://github.com) account, if you don’t have one already.
* Download Github desktop, set it up, and log into your account
* Install Homebrew
* Install Git

* Install Jekyll prerequisites
  * You can use the Jekyll Quickstart Guide to continue your installation (and troubleshoot issues); the below instructions duplicate those instructions, but are written in the context of this workshop:

* Install the Xcode Command Line Tools using your Terminal app.
```
xcode-select --install
```

* Install the macOS SDK headers:
```
open /Library/Developer/CommandLineTools/Packages/macOS_SDK_headers_for_macOS_10.14.pkg
```

* Install rbenv
  * follow install instructions for installing different versions and setting up rbenv in your shell, and install 2.7.2
  * run 
  ```rbenv local 2.7.2
  ``` 
  ...and then 
  ```
  rbenv local
  ``` 
  ...(should return this version number
  
* [Install gems](https://github.com/rbenv/rbenv#installing-ruby-gems) 
* Download / update Ruby gems: ```gem update --system```
* Install GCC
* Install Make
=======

# Welcome to Comitting to Documentation!

Instructors:
* Nick Krabbenhoeft
* Alison Rhonemus
* Genevieve Havemeyer-King

## Workshop pre-requisites
Please follow the below instrctuons prior to the workshop:

### Mac OS
* Install Visual Studio Code (https://code.visualstudio.com/) 
* Create a GitHub account.
* Download Github desktop, set it up, and log into your account
* Install Jekyll prerequisites
  * You can use the Jekyll Quickstart Guide to continue your installation (and troubleshoot issues); the below instructions duplicate those instructions, but are written in the context of this workshop:

Open a terminal window to continue with the following. 

* Install Homebrew 
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
* Install Git
*  [Install Ruby](https://jekyllrb.com/docs/installation/#requirements) - follow the guide for your operating system
  * Ruby install with [rbenv](https://github.com/rbenv/rbenv) is highly recommended
* Download / update Ruby gems: 
```
gem update --system
```
* Install [GCC](https://gcc.gnu.org/install/)
* Install [Make](https://www.gnu.org/software/make/)


* Install the jekyll and bundler gems.
```
gem install jekyll bundler
```


### Windows
...



>>>>>>> origin/gh-pages
