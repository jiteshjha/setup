# setup
 :relieved: Setting up development environment on Debian based distros 
 
 `Tested on Ubuntu 14.01 LTS and Mint 17.`
 
 
## System Update
---

    $ sudo apt-get update && sudo apt-get upgrade

---

## Text Editors

### Vim
    $ sudo apt-get install vim
    
### Atom

    $ sudo add-apt-repository ppa:webupd8team/atom
    $ sudo apt-get update
    $ sudo apt-get install atom
     
## Google chrome
    $ sudo add-apt-repository -y "deb http://dl.google.com/linux/chrome/deb/ stable main"
    $ sudo apt-get update
    $ sudo wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub
    $ sudo apt-get install google-chrome-stable

## vlc player
    $ sudo add-apt-repository -y ppa:n-muench/vlc
    $ sudo apt-get install vlc
    
## Dropbox
    $ sudo apt-get install nautilus-dropbox
## Adobe Flash Player
    $ sudo apt-get install flashplugin-installer 
    
## Git
    $ sudo apt-get update
    $ sudo apt-get install git
    $ git config --global user.name "Your Name"
    $ git config --global user.email "youremail@domain.com"

