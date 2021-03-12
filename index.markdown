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

| **Time** | **Activity** | **Notes** |
|   -----          |     -----      |     -----      |
|   1:00PM - 1:15AM EST      |  Welcome & Introductions |      Nick intros   |
|   1:15AM - #### EST        | GitHub Basics  |      Intro and usage   |
|   12:00PM - 12:15PM EST    |  Thinking about docs |     Notes about this     |
|   12:15PM - 12:45PM EST    |  Break |      Snack time!     |
|   1:15PM - 1:30PM EST      |  Writing docs: Markdown |      Notes about this   |
|   1:30PM - 2:00PM EST      |  Activity: Forking and committing |      Seems boring but it's not     |
|   2:00PM - 2:15PM EST      |  Site structuring  |      Notes about this     |
|   2:15PM - 2:45PM EST      |  Show n Tell |      Show us your docs!     |
