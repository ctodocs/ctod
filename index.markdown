---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
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