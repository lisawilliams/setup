# Setup Notes

## Overview

These are the setup notes for a new Mac laptop, purchased in May of 2022. It is a MacBook Air with a 265GB SSD drive and using Apple Silicon M1 processor. It's running MacOS 12.2.1 Monterey. (Note: during the install process for Ruby I updated the OS to give a clean start and it is now MacOS Monterey 12.4)



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
* After pushing repo, was able to find setup repo on Github: https://github.com/lisawilliams/setup/blob/main/setup_notes.md
* Installing Homebrew via the command line with the following command `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"` according to the homebrew homepage here https://brew.sh/ Not clear to me if you need to be in a specific dir to do that so I went cd ~ first. 
* That works but you need to `sudo` which is fine I guess. It downloads Command Line Tools for XCode. You would think with how big it is the CLI for XCode would come with but I guess not. 
* This also seems to take a minute. Back to *Years and Years.* 
* Homebrew installed but gave the following message `Warning: /opt/homebrew/bin is not in your PATH.` Helpful instructions gave a fix: Next steps: Run these two commands in your terminal to add Homebrew to your PATH: `echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/lisawilliams/.zprofile eval "$(/opt/homebrew/bin/brew shellenv)"`
* Having done that I ran `brew doctor` and recieved `Your system is ready to brew`
* I think I may leave install of Ruby and the other items on the Shopping List until tomorrow (it's actually already tomorrow but you know what I mean).

Sunday, June 5 2022

* Following the instructions [here](https://mac.install.guide/ruby/1.html) I updated MacOS. It is now Monterey 12.4. 
* I am using [Mac Install Guide: Ruby](https://mac.install.guide/ruby/) to use up-to-date Ruby rather than Mac system Ruby (which is old and may be deprecated soon).
* Installed `asdf`, a package manager for Ruby, using `homebrew`. Did this because `asdf` will let you manage multiple versions of Ruby. Not totally sure this is necessary for me...but the fact that I have system Ruby and want a current and updateable Ruby makes it seem like a goodish bet?
* Installed Ruby using `asdf` according to the instructions [here](https://mac.install.guide/ruby/6.html)
* `ruby -v` now returns Ruby 3.1.2p20 2022-04-12
* forked and cloned `lisa` and tested connection to github (success)





## Shopping list: 

* XCode DONE
* Sublime Text DONE
* Git/Github DONE 
* Homebrew DONE
* Install asdf for Ruby version management DONE
* Ruby 3.1.2 DONE
* fork/clone lisa and autolisa repos DONE
* Install Tableau and port license key and workbooks


Mon, Jun 24, 2024. I am following these notes once again to set up a new Mac laptop running iOS 14.3 (Sonoma).

* Laptop is set up. As usual I deferred Migration Assistant. 
* Tableau keys and workbooks were set up last week. 
* Downloaded and installed XCode (seemed to be much faster this time). 
* XCode appears to have installed Git. I was able to fork and clone the repo this note resides in. I will test it further to be sure I can also push changes to a repository on Github. 
* 