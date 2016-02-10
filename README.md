# setup
 :relieved: Setting up development environment on Debian based distros 
 
 `Tested on Ubuntu 15.04 LTS.`
 
 
## System Update
---

    $ sudo apt-get update && sudo apt-get upgrade

---

## WiFi Connection Error

    $ sudo service network-manager stop
    $ sudo gedit /etc/modprobe.d/iwlwifi.conf

Add options iwlwifi 11n_disable=1 to file, save, and close. Then:

    $ sudo rmmod iwlmvm iwlwifi 
    $ sudo modprobe iwlmvm iwlwifi 
    $ sudo service network-manager restart



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

## Synaptic Package Manager
    $ sudo apt-get install synaptic

## Deluge
    $ sudo apt-get install deluge

## Java 8
    $ sudo add-apt-repository ppa:webupd8team/java
    $ sudo apt-get update
    $ sudo apt-get install oracle-java8-installer
    $ java -version
    $ sudo apt-get install oracle-java8-set-default
   
## Unrar
    $ sudo apt-get install unrar
