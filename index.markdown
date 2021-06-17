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
* Install Visual Studio Code (https://code.visualstudio.com/) 
* Create a GitHub account.
* Download Github desktop, set it up, and log into your account
* Open a terminal window and continue with the following steps for your operating system.

### Mac OS

* Install Homebrew 
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
* Install Git: 
```
brew install git
```
*  Install [rbenv](https://github.com/rbenv/rbenv#installation)
```
brew install rbenv
```
* Set up rbenv for your shell:
```
rbenv init
```
* Setup your terminal to start rbenv on open:
```
echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
source ~/.bash_profile
```
* Check your installation (you should see a bunch of "OK"s)
```
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/main/bin/rbenv-doctor | bash
```
* Install Ruby 2.7.2 using rbenv, which is not the latest version, but is the version required for GitHub Pages.
```
rbenv install 2.7.2
```

* Set Ruby 2.7.2 as your global version
Note: This will set version 2.7.2 as your default Ruby version. If you're working on other Ruby projects with the computer you're using for this workshop, feel free to contact us for help maintaining multiple versions.
```
rbenv global 2.7.2
```
* Restart your terminal

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
* Download and install a Ruby+Devkit version from [RubyInstaller Downloads](https://rubyinstaller.org/downloads/). Use default options for installation.
* Run the `ridk install` step on the last stage of the installation wizard. This is needed for installing gems with native extensions. You can find additional information regarding this in the [RubyInstaller Documentation](https://github.com/oneclick/rubyinstaller2#using-the-installer-on-a-target-system)
* Open a new command prompt window from the start menu, so that changes to the PATH environment variable becomes effective. Install Jekyll and Bundler using `gem install jekyll bundler`




# Schedule

| **Time** | **Topic** | **Activity** |
|     -----          |     -----      |     -----      |
|   1:00 PM - 1:15 PM   |   Introductions |   Tell us about you   |
|   1:15 AM - 1:45 PM   |   Intro to Ruby, Jekyll, and GitHub   |   Commit, Fork & Serve   |
|   1:45 PM - 2:15 PM   |  Writing documentation |     Planning and drafting      |
|   2:15 PM - 2:30 PM   |  Mini Break |      Eat snacks!     |
|   2:30 PM - 3:00 PM   |  Writing in Markdown   |      Converting notes to a doc   |
|   3:00PM - 3:30PM   |  Site structure |      Organizing and connecting docs     |
|   3:30PM - 3:45PM   |  Break #2 |      Move around!     |
|   3:45PM - 4:15PM   |   Collaboration  |     Contributing edits to others' docs    |
|   4:15PM - 5:00PM   |  Show n Tell / Q & A |      Share your docs     |
