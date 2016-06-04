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


## Python 2.7
    $ sudo apt-get install build-essential checkinstall
    $ sudo apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev
    $ sudo add-apt-repository ppa:fkrull/deadsnakes
    $ sudo apt-get update
    $ sudo apt-get install python2.7

## pip
    $ sudo apt-get install python-pip

## flask
    $ sudo pip install flask
    
## Oracle SQL
    User : SYSTEM
    Pass : Password

## Public Lab's plots2 installation
- Fork the repo on Github, and on c9.io create a new workspace with "blank" as an option.
- Run ``` ./install_cloudnine.sh ``` on terminal in c9
- Copy [this](https://gist.github.com/jiteshjha/714bd2e528e789c7057d4bacaa8a3364 to database.yml) (NOTE: Leave the password field as it is and mind the indentation), and copy schema.rb.example to schema.rb
- ``` rvm use ruby-2.1.2 ```
- ```mysql-ctl start```
- ``` rake db:create ```
- ``` rake db:setup ```
- ``` rake db:migrate ```


