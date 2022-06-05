# Setup Notes

## Overview

These are the setup notes for a new Mac laptop, purchased in May of 2022. It is a MacBook Air with a 265GB SSD drive and using Apple Silicon M1 processor. It's running MacOS 12.2.1 Monterey. 

These are the steps I took to create a working development environment. -- Lisa Williams, Saturday June 4, 11:55 PM

* Opened laptop, powered it on, went through Mac setup process. Opted out of Migration Assistant for now. 
* Downloaded Chrome, mainly for access to online accounts. 
* Created /code directory: Created /code directory under /lisawilliams/ user directory. 
* Created /setup directory in the /code directory and created setup_notes.md to document my process. 
* Downloaded Sublime Text. 
* Tested opening folders and files in Sublime Text from the Terminal. `open -a "sublime text" [filename or foldername]` works. In order to open a folder you must be in its parent folder, not in the folder itself. 
* Went to the Apple App store and began downloading XCode. This thing is huge and takes forever. 
* Watched more of "Sort Of" on HBO Max while XCode downloaded. 
* Looked at GA's Installfest repo. Reluctant to use it verbatim as it has not been updated since 2017, but the general outline still seems helpful. https://github.com/ga-wdi-boston/orientation/blob/master/INSTALLFEST.md 
* [Why does XCode Take Forever To Install?](https://www.swiftdevjournal.com/xcode-installation-questions/#:~:text=Why%20does%20Xcode%20take%20forever,2%20hours%20to%20install%20Xcode.) 
* Have watched the entirety of the delightful Sort Of and have moved on to Years And Years, bless the HBO Max pride month lineup. `update: not sure I should be watching Years and Years, I think it might be too scary`
* Once I've got Git installed and set up, I want to install Ruby instead of using Mac system Ruby. [Mac system Ruby isn't up to date and is due to be deprecated anyway](https://www.freecodecamp.org/news/do-not-use-mac-system-ruby-do-this-instead/). Good instructions for installing up to date Ruby are here. [InstallGuide, Ruby on MacOS](https://mac.install.guide/ruby/index.html). 
* XCode is installed. `git status` returns `fatal: not a git repository` which I suppose means git is there
* Set my git username via these instructions https://docs.github.com/en/get-started/getting-started-with-git/setting-your-username-in-git
* Began the process of setting up git and connecting it to github via these instructions: https://kbroman.org/github_tutorial/pages/first_time.html
* * Ran `git init` in `setup`, added files, wrote commit message, pushed (but failed)
* Got stopped because the instructions assume a username/password for github from the command line. Github now uses personal access tokens. I generated a new token using these instructions, saved it to my github account, and was able to push my local repo to github. https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token



## Shopping list: 

* XCode
* Sublime Text
* Git/Github
* Homebrew
* Ruby 3.0
* fork/clone lisa and autolisa repos
* Install Tableau and port license key and workbooks