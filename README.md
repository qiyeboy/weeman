Weeman - http server for phishing
=================================

About
=====

I wrote this as a tool to test network security (the users),
Usually we will run Weeman with dns spoof attack (MITM).

Weeman will do the following steps:
------------------------------------

1. Create fake html page.
2. Wait for clients
3. Grab the data (POST).
4. Try to login the client to the original page :smiley:

![Weeman](https://raw.githubusercontent.com/Hypsurus/weeman/master/core/weeman12.png)

Requirements
============

* Python <= 2.7
* Python BeautifulSoup 4

Install BeautifulSoup
---------------------

* Archlinux        - sudo pacman -S python2-beautifulsoup4
* Ubuntu/Linuxmint - sudo apt-get install python-bs4
* For another OS:  - sudo pip install beautifulsoup4

Platforms
-----------

* Linux (any)
* Mac (Not tested)
* Windows (Not tested)

If weeman runs on your platform (Mac/Windows), please let me know.

Usage
======

Just type `help`

Run server:
-----------

* For port 80 you need to run Weeman as root!

* Host to clone (Ex: www.social-networks.local)
> set url http://localhost

* "<code><"form action = "TAKE THIS URL">"</code>(View the site source and take the URL)
> set action_url http://localhost/sendlogin 

* The port Weeman server will listen
> set port 2020

* Start the server
> run

Get Weeman
=============
                git clone git://github.com/Hypsurus/weeman
  
Copyright 2015 (C) Hypsurus <hypsurus@mail.ru>.

License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>.
