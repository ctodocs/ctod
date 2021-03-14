---
title: Welcome
layout: default
nav_order: 1
---

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
* Install Git: 
```
brew install git
```
*  [Install rbenv](https://github.com/rbenv/rbenv#installation)
```
brew install rbenv
```
  * set up rbenv for your shell; follow the printed commands after running...:
  ```
  rbenv init
  ```
* Check your installation
```
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash
```
* Install Ruby 2.7.2 using rbenv, which is not the latest version, but is the version required for GitHub Pages.
```
rbenv install 2.7.2
```

* Set Ruby 2.7.2 as your global version
```
rbenv global 2.7.2
```

* Download / update Ruby gems: 
```
gem update --system
```

* Install the jekyll and bundler gems.
```
gem install jekyll bundler
```

#### Things you may/may not need to install depending on your system defaults:
* Install [GCC](https://gcc.gnu.org/install/)
* Install [Make](https://www.gnu.org/software/make/)


### Windows
...




# Schedule

| **Time** | **Topic** | **Activity** |
|     -----          |     -----      |     -----      |
|   1:00 PM - 1:15 PM       |  Introductions |      Tell us about you   |
|   1:15 AM - 1:45 PM         |   Intro to Ruby, Jekyll, and GitHub  |     Fork & Serve   
|   1:45 PM - 2:15 PM     |  Writing documentation |     Planning and drafting      |
|   2:15 PM - 2:30 PM   |  Mini Break |      Eat snacks!     |
|   2:30 PM - 3:00 PM   |  Writing in Markdown   |      Converting notes to a doc   |
|   3:00PM - 3:30PM   |  Site structure |      Organizing and connecting docs     |
|   3:30PM - 3:45PM   |  Break #2 |      Move around!     |
|   3:45PM - 4:15PM   |   Collaboration  |     Contributing edits to others' docs    |
|   4:15PM - 5:00PM   |  Show n Tell / Q & A |      Share your docs     |
