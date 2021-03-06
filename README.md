<h1><img src="https://raw.githubusercontent.com/tim-sueberkrueb/ubuntu-hangups/master/ubuntu-hangups.png" width="64"> Ubuntu Hangups</h1>


An unofficial Google Hangouts client for Ubuntu Touch

This application uses <a href='https://github.com/tdryer'>Tom Dryer</a>'s unofficial Google Hangouts Python library <a href='https://github.com/tdryer/hangups'>Hangups</a>.
Powered by <a href='https://github.com/thp'>Thomas Perl's</a> <a href='https://github.com/thp/pyotherside'>PyOtherSide</a>

## Third-party software
Ubuntu Hangups includes the following third-party software:
* Notification sound (media/notification-sound.wav) by TheGertz is licensed under the Creative Commons 0 License (cc-0, http://creativecommons.org/publicdomain/zero/1.0/): https://www.freesound.org/people/TheGertz/sounds/235911/
* Send icon from Googles Material Design icons (media/google-md-send-icon.svg) is licensed under the Creative Commons Attribution-Share Alike 3.0 Unported License (CC BY SA 3.0): https://design.google.com/
* The loading animation (media/loading-animation.gif) by Fabian Süberkrüb is licensed under the Creative Commons Attribution License 4.0 (CC BY 4.0, https://creativecommons.org/licenses/by/4.0/)
* The default chat background (media/default_chat_wallpaper.jpg) was created by Patrick Hoesly and is licensed under the Creative Commons Attribution 2.0 Generic (CC BY 2.0) license.

The application icon was created by <a href="http://samuelhewitt.com/">Sam Hewitt</a>, thanks so much :)

## Translations
Ubuntu Hangups is on Transifex! Please help me translating this app and contribute:

https://www.transifex.com/tim-sueberkrueb/ubuntu-hangups/

## Contact
Contact me via Gitter: https://gitter.im/tim-sueberkrueb/

# Installation on Ubuntu

## Dependencies
* ubuntu-ui-toolkit 1.3
* pyotherside (https://thp.io/2011/pyotherside/)
* hangups (https://github.com/tdryer/hangups)
  * aiohttp
  * purplex
  * requests
  * reparser
  * google.protobuf
* pymmh3 (or another python MurmurHash3 implementation, e.g. mmh3)
* dateutil

## Install and run on Ubuntu Desktop

Clone ubuntu-hangups

```
git clone https://github.com/tim-sueberkrueb/ubuntu-hangups
```

### Installation
* Install PyOtherSide

 ```
  sudo apt-get install pyotherside
  ```
* Download and install hangups

  ```
  pip3 install hangups
  ```
* Install a MurmurHash3 implementation

  ```
  sudo pip3 install mmh3
  ```
* Make sure that all python dependencies (see above) are installed.

### Run
Inside the ubuntu-hangups directory run:

```
qmlscene Main.qml
```


## Build for Ubuntu Touch
* Make sure you have the Ubuntu SDK installed

  https://developer.ubuntu.com/en/start/ubuntu-sdk/installing-the-sdk/

* In order to get the dependencies run from the ubuntu-hangups directory:

 `git submodule update --init --recursive` 


### Build and run
* Open ubuntu-hangups.qmlproject with the Ubuntu-SDK, add the appropriate build kit and run!


## Copyright and License
(C) Copyright 2015-2016 by Tim Süberkrüb and contributors

See CONTRIBUTORS.md for a full list of contributors.

This application is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

See LICENSE for more information.

This application is not endorsed by or affiliated with Ubuntu or Canonical. Ubuntu and Canonical are registered trademarks of Canonical Ltd.
